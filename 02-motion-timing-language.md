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

### Page Load - "Intelligence World"
- Delay: 150ms after load.
- Sequence:
  1. Depth grid fade in (300ms).
  2. Layer planes appear (500ms).
  3. Inference core forms (900ms).
  4. Data streams fall into the core (1200ms).
  5. Decision wave spreads across the horizon (600ms).
  6. Headline reveal (320ms).
- Total: 2.4s to 3.0s.

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

### Hero World Engine (Home)
- Camera drift: 12-16s loop, 1-2 degrees orbit.
- Depth parallax: 2-4px per layer.
- Inference core pulse: 4-6s loop, soft glow.
- Ripple interaction: 240ms start, 800ms decay.
- Scroll tilt: 6 degrees over 600ms.

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

### System Atlas Cards
- Cluster reveal: 420ms with 60ms stagger.
- Hover highlight: 160ms glow in, 160ms glow out.
- Connection line draw: 240ms linear.

### Pipelines and Diagrams
- Stage activation: 240ms per node.
- Sequence: 80ms delay between nodes.
- Use accent only on the active stage.

### Agentic Orchestration Diagram
- Role lattice orbit: 10-14s loop, 1-2 degrees rotation.
- Message packet flow: 600-900ms travel, 2-3s interval.
- Consensus ring pulse: 420ms in, 600ms out.
- Task queue tick: 280ms reveal per item, 80ms stagger.
- Tool gate flash: 120ms amber, 300ms fade.

### Tool Invocation Trace Mesh
- Trace line draw: 220-320ms linear.
- Trace ID label fade: 180ms in, 600ms out.
- Policy stamp: 140ms pop, 240ms fade.
- Trace expiry: 1.2-1.8s dissolve.

### Conflict Resolution Flow
- Conflict flag: 120ms amber in, 400ms hold, 300ms out.
- Split path reveal: 260ms each branch, 80ms stagger.
- Resolution merge: 320ms, soft ease.
- Reason code type-in: 20-30ms per character.

### Architecture Blueprint Diagram
- Layer highlight: 200-260ms.
- Stack flow line: 1.0-1.4s linear.
- Variant toggle swap: 220-320ms.

### RAG Pipeline Diagram
- Step highlight: 220-300ms.
- Retrieval pulse: 600-800ms.
- Citation attach line: 200-260ms.

### Social Connectivity Map
- Channel glow: 160-220ms.
- Normalization converge: 420-520ms.
- Routing branch draw: 260-340ms.

### Vision Detection Pipeline
- Frame capture pulse: 200-260ms.
- Detection sweep: 520-680ms.
- Threshold line flash: 120ms amber, 300ms fade.

### Impact and ROI Estimator
- Slider response: 120-180ms.
- Range band update: 200-260ms.
- Confidence band fade: 260-320ms.

### Metrics Dashboard
- Metric tick update: 180-240ms.
- Threshold flash: 120ms amber, 300ms fade.
- Drift indicator pulse: 600ms loop, low intensity.

### Procurement Pack Access
- Document list reveal: 160-220ms stagger.
- Access panel swap: 200-260ms.

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
