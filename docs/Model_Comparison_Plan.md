# Model Comparison Plan

## Purpose

This experiment does not attempt to prove which model is universally best.

It tests which model best supports the AI Craypas experience:

> Generating understandable, surprising, cross-domain, multi-hop pathways between two selected concepts.

---

## Models

Initial comparison candidates:

- Gemini
- Claude
- GPT-family model

Perplexity should not be used as a primary comparison model because search retrieval may affect its output style and factual grounding.

It can be tested separately as a possible verification layer.

---

## Test Rules

Every model should receive:

- The same input pair
- The same prompt
- The same requested output structure
- The same language
- The same maximum number of hops

Each input pair should be tested at least three times per model.

A single strong output should not be treated as representative.

---

## Test Input Pairs

### 1. Fact and Geography

Input pair:

    Fingernail → Magellan

What to evaluate:

- Biological and geological reasoning
- Geographic accuracy
- Historical connection quality

---

### 2. Cross-Domain Connection

Input pair:

    Alleyway → Glacier

What to evaluate:

- Ability to move across ecology, physics, geography, urban structure, or language
- Ability to maintain a coherent route
- Ability to generate more than one meaningful route

---

### 3. Culture and Technology

Input pair:

    Frieren → Post-it

What to evaluate:

- Cultural interpretation
- Information and memory connection
- Avoidance of forced media references

---

### 4. Biology and Space

Input pair:

    Orchid → Voyager

What to evaluate:

- Biological signaling
- Communication systems
- Cross-domain structural reasoning

---

### 5. Difficult Random Pair

Input pair:

    Crane → Black Hole

What to evaluate:

- Ability to avoid arbitrary connection
- Willingness to reject a weak path
- Quality of structural analogy when direct factual links are unavailable

---

## Common Prompt Template

Use the following prompt for every model.

    Generate an understandable multi-hop conceptual pathway between Concept A and Concept B.

    Rules:

    - Use 4 to 6 pathway nodes.
    - Every hop must clearly connect to both the previous and next concept.
    - Label each hop as one of:
      [Fact]
      [Structural Analogy]
      [Cultural Connection]
    - Do not present analogy as factual evidence.
    - Avoid wordplay, sound similarity, or arbitrary associations.
    - If a strong pathway cannot be formed, say so instead of forcing one.
    - Identify claims that require fact verification.

    Output format:

    1. Pathway nodes
    2. One-line explanation for every hop
    3. Connection type tags
    4. One short discovery insight
    5. Claims requiring verification

---

## Evaluation Rubric

Score every output from 1 to 5.

| Criterion | Evaluation Question |
|---|---|
| Endpoint Validity | Does the path genuinely reach Concept B from Concept A? |
| Hop Density | Is each step understandable without abrupt jumps? |
| Cross-Domain Quality | Does the pathway move between domains naturally? |
| Structured Surprise | Does the complete pathway create a convincing “I would not have connected these before” moment? |
| Intermediate Discovery Value | Do the intermediate nodes reveal unfamiliar, meaningful, or reusable words, facts, domains, or perspectives? |
| Factual Stability | Are factual claims likely to be accurate and checkable? |
| Product Readability | Can the output be shown as clean, understandable cards in an app? |

### Structured Surprise

This criterion evaluates the complete pathway.

A strong result should make the evaluator feel:

> “I would not have connected these two concepts before, but now I understand why.”

The score should reflect both:

- the unexpectedness of the endpoint connection
- the coherence of the full route

A surprising but arbitrary route should not receive a high score.

### Intermediate Discovery Value

This criterion evaluates what the user discovers before reaching the endpoint.

Strong intermediate nodes may provide:

- an unfamiliar word
- a previously unknown fact
- a new domain
- a different perspective on a familiar concept
- a concept worth saving or reusing later

Intermediate nodes should not exist only to fill the distance between the endpoints.

> Each intermediate node should have the potential to become a small discovery.


---

## Evaluation Notes

When comparing outputs, model names should be hidden during first-pass scoring.

For example:

- Output A
- Output B
- Output C

This reduces the chance of favoring a model because of prior expectations.

After scoring, reveal the model names and compare patterns across runs.

---

## Interpretation

### When one model repeatedly performs better

Do not claim universal superiority.

Use wording such as:

> In early exploratory tests, this model often produced more coherent and cross-domain conceptual pathways for this specific interaction.

### When all models perform similarly

The core product value may depend more on:

- Prompt design
- Grounding and verification
- Path evaluation
- Fact and analogy distinction
- Interaction design
- Sketchbook experience

### When outputs are surprising but unreliable

The product needs a stronger grounding and verification layer before it can claim educational value.

---

## Comparison Table

Use the following table after testing.

| Input Pair | Model | Run | Endpoint Validity | Hop Density | Cross-Domain Quality | Structured Surprise | Intermediate Discovery Value | Factual Stability | Product Readability | Notes |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---|
| Fingernail → Magellan | Gemini | 1 |  |  |  |  |  |  |  |
| Fingernail → Magellan | Claude | 1 |  |  |  |  |  |  |  |
| Fingernail → Magellan | GPT | 1 |  |  |  |  |  |  |  |
| Alleyway → Glacier | Gemini | 1 |  |  |  |  |  |  |  |
| Alleyway → Glacier | Claude | 1 |  |  |  |  |  |  |  |
| Alleyway → Glacier | GPT | 1 |  |  |  |  |  |  |  |
| Frieren → Post-it | Gemini | 1 |  |  |  |  |  |  |  |
| Frieren → Post-it | Claude | 1 |  |  |  |  |  |  |  |
| Frieren → Post-it | GPT | 1 |  |  |  |  |  |  |  |
| Orchid → Voyager | Gemini | 1 |  |  |  |  |  |  |  |
| Orchid → Voyager | Claude | 1 |  |  |  |  |  |  |  |
| Orchid → Voyager | GPT | 1 |  |  |  |  |  |  |  |
| Crane → Black Hole | Gemini | 1 |  |  |  |  |  |  |  |
| Crane → Black Hole | Claude | 1 |  |  |  |  |  |  |  |
| Crane → Black Hole | GPT | 1 |  |  |  |  |  |  |  |

---

## Deliverable

At the end of the experiment, summarize:

1. Which model produced the strongest pathways most consistently
2. Which input pairs were difficult for all models
3. Which kinds of errors appeared most often
4. Whether a grounding layer is necessary for the prototype
5. What the final AI Craypas prompt and interface need to emphasize
6. Which models most consistently produced valuable intermediate discoveries rather than merely completing the endpoint connection
