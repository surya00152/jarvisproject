# Page Prompt: RAG System Blueprint

This page explains a full Retrieval Augmented Generation system as a clean, technical pattern. It must feel like an engineering blueprint, not a sales pitch.

## Page Intent
- Make RAG concrete and trustworthy for technical and non-technical readers.
- Show how retrieval, memory, and reasoning connect safely.
- Highlight quality controls without hype.

## CTA Strategy (page level)
- Primary CTA: "Ask the AI to map this to your data" (voice).
- Secondary CTA: "See the reference architecture".

---

## Section 1: RAG Hero
**Purpose**
- Define the RAG pattern in one simple frame.

**Content Intent**
- Headline: "Retrieval, then reasoning."
- Subtext: "Grounded answers from your knowledge base."

**Design and Animation Logic**
- A minimal pipeline diagram with a single flow line.

---

## Section 2: RAG Pipeline (Primary Diagram)
**Purpose**
- Show the full flow from documents to responses.

**Content Intent**
- Steps:
  1. Ingest and normalize content
  2. Chunk and embed
  3. Vector search retrieval
  4. Context assembly
  5. Reasoning and response
  6. Citation and trace

**Design and Animation Logic**
- Each step lights in sequence with short labels.
- A trace line shows where citations are attached.

---

## Section 3: Retrieval Quality Controls
**Purpose**
- Explain how relevance and precision are maintained.

**Content Intent**
- Re-ranking and relevance scoring.
- Query expansion and filtering.
- Human review for critical outputs.

**Design and Animation Logic**
- A filtering gate that tightens the signal.

---

## Section 4: Grounding and Citations
**Purpose**
- Show how responses stay tied to sources.

**Content Intent**
- "Every response points to its source."
- "No source, no claim."

**Design and Animation Logic**
- A citation line attaches to each output node.

---

## Section 5: Memory and Updates
**Purpose**
- Clarify how knowledge stays current.

**Content Intent**
- Incremental updates and re-indexing.
- Clear retention and deletion rules.

**Design and Animation Logic**
- A loop from "new content" back into the index.

---

## Section 6: Conversion Panel
**Purpose**
- Encourage a focused technical conversation.

**Content Intent**
- "Tell the AI where your knowledge lives."

**CTA Placement**
- Primary: "Ask the AI to map this to your data" (voice).
- Secondary: "See the reference architecture".

**AI Voice Assistant Integration**
- Launch external voice app with context: "RAG -> Data mapping".
