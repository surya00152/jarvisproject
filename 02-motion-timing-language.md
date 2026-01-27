# Motion and Timing Language - AI Interface System

This document defines the animation and interaction timing for the entire site. Motion must feel precise, intelligent, and calm. Avoid playful or chaotic movement.

## Motion Intent
- Motion implies data flow, inference, and decisioning.
- Every animation should have a purpose.
- No continuous busy animation. Use slow, breathing loops.

## Timing Tokens
- Micro: 120-180ms (button hover, icon shift)
- Short: 200-260ms (card hover, small reveals)
- Medium: 280-420ms (section reveals, toggles)
- Long: 600-900ms (system map focus, diagram flow)
- Extra long: 1200-2000ms (awakening sequences, neural formation)

## Easing Curves
- Standard: cubic-bezier(0.2, 0.8, 0.2, 1)
- Soft: cubic-bezier(0.16, 1, 0.3, 1)
- Precise: cubic-bezier(0.3, 0.7, 0.1, 1)
- Linear: for data flow lines only

## Motion Scale
- Translate: 6-12px for micro, 16-24px for section reveals.
- Opacity: 0.0 -> 1.0 with no overshoot.
- Blur: max 6px on entrance only, never on text.

## Global Sequences

### Page Load - "AI Awakening"
- Delay: 150ms after load.
- Sequence:
  1. Background grid fade in (300ms).
  2. Neural points appear (600ms).
  3. Data lines connect (900ms).
  4. Headline reveal (320ms).
- Total: 1.8s to 2.2s.

### Scroll Reveal
- Offset: 40-60px upward.
- Opacity: 0 to 1.
- Duration: 280-360ms.
- Stagger: 60-90ms between items.

### System Logs
- Type-in effect: 20-30ms per character.
- Cursor blink: 600ms on, 600ms off.
- Auto-fade after 4-6s.

## Component Motion Specs

### Voice Assistant Orb
- Idle pulse: 4-6s loop, 6 percent scale, 10 percent glow.
- Hover: 160ms scale up, 10 percent glow increase.
- Listening: 300ms pulse cadence, teal accent active.
- Thinking: slow gradient shimmer, 1.8s cycle.
- Speaking: waveform ripple, 600ms loop.

### Capability Cards
- Hover lift: 6-8px, 180ms.
- Expand: 320-420ms with height and opacity.
- Technical toggle: 200ms fade and slide.

### System Map
- Node focus: 300ms glow in, 300ms glow out.
- Connection flow: 1.2s line travel, 4s interval.
- Hover: connected nodes highlight at 50 percent intensity.

### Demo Tiles
- Hover: status LED pulses once (200ms).
- CTA focus ring: 180ms.
- Launch transition: 600ms fade to dark before external open.

### Scenario Cards
- Hover: signal pulse along the card edge (240ms).
- Expand: 360ms, show system stack.

### Pipelines and Diagrams
- Stage activation: 240ms per node.
- Sequence: 80ms delay between nodes.
- Use accent only on the active stage.

### Trust and Policy Pages
- Minimal motion only.
- Use amber highlight for checks (120ms flash, 300ms fade).

## Gradient Rules
- Gradients appear only during "thinking" states.
- Do not use gradients for static backgrounds.

## Sound Guidelines (Optional)
- Use soft, short cues only on state changes.
- Listening start: single soft tone (subtle).
- Thinking start: low pulse (subtle).
- Speaking: no sound cues.
- Provide a global toggle for audio.

## Reduced Motion Mode
- Disable loops and background flows.
- Replace motion with static highlights.
- Keep only essential state changes (opacity only).
