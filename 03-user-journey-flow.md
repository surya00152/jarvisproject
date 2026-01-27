# User Journey Flow - AI Interface Experience

This document defines the full user journey flows and routing logic. The experience must feel like an intelligent system guiding the visitor, not a traditional marketing funnel.

## Global Journey Principles
- Lead with intelligence, not sales.
- Voice is the primary conversion path.
- Demos are proof, not persuasion.
- System trust pages are accessible without breaking flow.
- Every page offers a clear next step (voice, demo, or diagnostic).

## Primary Journeys (Entry to Conversion)

### Flow A: Voice-First (Default)
**Entry points**
- Home hero CTA, persistent voice orb, Talk to the AI page.

**Path**
1. Home hero: "Ask the AI"
2. Voice assistant qualifies the scenario
3. AI proposes a system path (capabilities + process)
4. If aligned, route to next step: pilot or scheduling

**Exit**
- Talk to the AI (contact) or Engagement Model page.

---

### Flow B: Demo-First (Curiosity to Proof)
**Entry points**
- Home demo tiles, Live AI Experiences page, capability cards.

**Path**
1. Demo selection (no sign-up)
2. After demo: "Ask the AI what you just saw"
3. AI explains the system behind the demo
4. Route to capability or process page

**Exit**
- Voice assistant qualification or readiness diagnostic.

---

### Flow C: Capability-First (Technical Buyer)
**Entry points**
- AI Capabilities page, system map link.

**Path**
1. Capability explorer (human problem -> AI approach)
2. Technical toggle reveals architecture hints
3. System map reinforces capability relationships
4. CTA: "Design my system with the AI"

**Exit**
- Voice assistant or process page.

---

### Flow D: Scenario-First (Non-Technical Buyer)
**Entry points**
- Industries and Use Scenarios page.

**Path**
1. Choose scenario
2. System suggests capabilities
3. Offer matching demo
4. Voice assistant asks 2-3 clarifying questions

**Exit**
- Readiness diagnostic or Talk to the AI.

---

### Flow E: Trust-First (Enterprise or Risk-Aware)
**Entry points**
- Privacy and Ethics, Security and Compliance, Monitoring and Support,
  Model Evaluation and Safety Metrics, Procurement FAQ, Procurement Pack.

**Path**
1. Read trust policy
2. Review evaluation metrics and safeguards
3. System suggests readiness diagnostic
4. Offer AI Architect for security questions

**Exit**
- Engagement model or voice assistant.

---

### Flow F: Research-First (Innovation-Driven)
**Entry points**
- System Status and Research Log.

**Path**
1. Review recent intelligence updates
2. "Ask the AI to explain the latest update"
3. AI connects updates to user scenario

**Exit**
- Demo hub or voice assistant.

---

### Flow G: Agentic-First (Advanced Technical Buyer)
**Entry points**
- Agentic Tech Flow page, process page, capability details.

**Path**
1. Review the agentic loop and tool orchestration
2. Inspect safety, control, and auditability
3. Ask the AI to map agentic tasks to their workflow

**Exit**
- Process page or voice assistant qualification.

---

### Flow H: Procurement-First (Legal or Procurement Teams)
**Entry points**
- Procurement FAQ, Procurement Pack, Security and Compliance.

**Path**
1. Read procurement Q and A
2. Review pack contents or request delivery
3. Ask the AI to clarify any open questions

**Exit**
- Engagement model or voice assistant.

---

### Flow I: Architecture-First (Technical Architecture Review)
**Entry points**
- Reference Architecture Blueprint, Integrations and Data Sources.

**Path**
1. Review the canonical stack
2. Toggle system variants (voice, vision, agentic)
3. Ask the AI to map to their environment

**Exit**
- Integrations page or voice assistant.

---

### Flow J: Pattern-First (System Pattern Review)
**Entry points**
- RAG System Blueprint, Social Message Connectivity, Vision Detection Pipeline.

**Path**
1. Review a system pattern
2. Map pattern to data or channels
3. Ask the AI for architecture fit

**Exit**
- Reference architecture or voice assistant.

---

## Routing Rules and Triggers

### CTA Routing Logic
- If user spends time in Capabilities: offer "Design my system".
- If user watches a demo: offer "Explain the system behind this".
- If user visits trust pages: offer "Ask about security".
- If user hits the process page: offer "Start a pilot".
- If user visits procurement pages: offer "Request the procurement pack".
- If user visits the blueprint: offer "Map this to my stack".
- If user visits the estimator: offer "Run readiness diagnostic".
- If user visits metrics: offer "Ask about evaluation and safety".
- If user visits a pattern page: offer "Map this to my data".

### Voice Assistant Context Tags
- Home -> "Entry"
- Capabilities -> "System design"
- Process -> "Build pipeline"
- Agentic -> "Agentic architecture"
- Demos -> "Experience explanation"
- Scenarios -> "Qualification"
- Trust pages -> "Risk and governance"
- Contact -> "Handoff"
- Procurement FAQ -> "Procurement Q and A"
- Procurement Pack -> "Procurement pack"
- Architecture Blueprint -> "Architecture mapping"
- Impact Estimator -> "Impact estimator"
- Change Management -> "Adoption"
- Model Evaluation -> "Metrics inquiry"
- RAG Blueprint -> "RAG mapping"
- Social Connectivity -> "Channel mapping"
- Vision Pipeline -> "Vision pipeline"

### Demo Recommendation Logic
- Voice or chat identifies a scenario.
- System recommends 1-2 relevant demos.
- The CTA uses the phrasing: "See intelligence in action".

### Readiness Diagnostic Logic
- Offer after 2 or more page interactions without conversion.
- Offer immediately on trust pages.
- After diagnostic, route to pilot or data mapping.

---

## Page-to-Page Transition Rules
- Keep flow linear for non-technical visitors (Home -> Scenarios -> Diagnostic -> Voice).
- Allow fast jumps for technical visitors (Home -> Capabilities -> Process -> Engagement).
- Trust and policy pages never dead-end; always route back to voice.

---

## Primary Conversion Paths (Summary)
- Voice Architect path: 60 percent of conversions.
- Demo path: 25 percent of conversions.
- Diagnostic path: 15 percent of conversions.

These are guidance targets, not strict constraints.
