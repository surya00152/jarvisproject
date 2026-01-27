# Next.js Implementation Plan - R3F + GSAP + Custom Shaders

This document defines SSR strategy, lazy loading, and performance practices for a Next.js site that uses React Three Fiber, GSAP, and custom shaders. It focuses on speed, stability, and Google PageSpeed Insights.

## Goals
- Keep the AI world hero cinematic without blocking LCP.
- Preserve smooth motion while minimizing CPU and GPU load.
- Deliver strong PageSpeed scores for both mobile and desktop.

## Stack Summary
- React Three Fiber (R3F) + Drei for 3D scenes.
- GSAP + ScrollTrigger for timeline and scroll choreography.
- Custom shaders for "intelligence world" visuals.
- SVG + GSAP for diagrams (agentic flows, system maps).

---

## SSR Strategy (Next.js App Router)
**Reality:** WebGL cannot SSR. The hero must be client-only with a server fallback.

**Plan**
1. Keep pages as server components by default.
2. Isolate 3D canvas and GSAP animations in small client components.
3. Use `next/dynamic` with `ssr: false` for the 3D hero and heavy animation modules.
4. Provide a server-rendered fallback for the hero:
   - Static poster image (optimized) with the same headline and CTA.
   - Reserve the final layout size to prevent CLS.
5. Hydrate the 3D scene after initial render with a progressive load.

**Example pattern**
- Server: `<HeroFallback />` for LCP.
- Client: `<HeroWorld />` loaded via dynamic import and swapped in after idle.

---

## Lazy Loading and Progressive Enhancement
**R3F**
- Load the 3D hero after LCP using `requestIdleCallback` or a short delay.
- Use `IntersectionObserver` for below-the-fold 3D or heavy diagrams.
- Defer non-critical shader layers until the first interaction.

**GSAP**
- Dynamically import GSAP and ScrollTrigger only when needed.
- Do not load ScrollTrigger on pages that do not use scroll animations.

**Images and Media**
- Use `next/image` for all raster assets.
- Use `priority` only for the hero fallback image.
- Prefer AVIF or WebP.

---

## Performance Guardrails (R3F and Shaders)
**Quality tiers**
- Detect device tier (GPU and memory) and adjust:
  - `dpr` capped at 1.0 to 1.5 on mobile.
  - Reduced particle count and lower shader complexity on low tier.

**Scene rules**
- Keep draw calls low (instancing for particles).
- Reuse geometries and materials via `useMemo`.
- Avoid large shadow maps and heavy post-processing on mobile.
- Use `frameloop="demand"` for static sections.

**Shader rules**
- Avoid large loops in fragment shaders.
- Use precomputed noise textures when possible.
- Share uniforms and materials across similar objects.
- Limit multi-pass effects.

---

## GSAP Integration Rules
- Register plugins only on the client.
- Use `gsap.context` inside `useLayoutEffect`.
- Clean up on unmount to avoid memory leaks.
- Respect `prefers-reduced-motion` and disable complex timelines.

---

## Google PageSpeed Insights Plan

### LCP (Largest Contentful Paint)
- LCP should be the static hero fallback, not the WebGL canvas.
- Preload fonts with `next/font` and limit font weights.
- Avoid any blocking JS before the hero text renders.

### INP (Interaction to Next Paint)
- Reduce JS on the critical path.
- Split animation code by route.
- Throttle heavy pointer handlers and avoid global listeners.

### CLS (Cumulative Layout Shift)
- Reserve fixed space for the hero and system atlas grid.
- Define image sizes and use aspect ratios.
- Avoid late-loading UI that pushes content.

### General PSI Tactics
- Use server components for all static content.
- Keep `use client` scope small and isolated.
- Compress JS and avoid large dependencies in the main bundle.
- Use route-based code splitting and dynamic imports.
- Cache static assets with long TTL.

---

## Suggested Implementation Steps
1. Build the hero fallback (static) for LCP.
2. Implement the R3F hero as a client component with dynamic import.
3. Add GSAP timelines only where required.
4. Add device-tier quality switching for R3F.
5. Add reduced-motion support globally.
6. Run Lighthouse and Web Vitals, then tighten bundles.

---

## Outcome Targets
- LCP < 2.5s on mobile (hero fallback).
- CLS < 0.1 site-wide.
- INP < 200ms for all primary interactions.

These targets are practical if the 3D layer is loaded after LCP.
