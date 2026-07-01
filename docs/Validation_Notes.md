# Validation Notes

## Current Research Question

Does a mainstream consumer experience already exist that allows users to choose two arbitrary concepts and receive an explainable, multi-hop pathway between them?

The pathway should prioritize:

- Understandability
- Cross-domain movement
- Structured surprise
- Clear distinction between facts and analogies
- A saveable discovery experience

---

## Adjacent References

### 1. Concept Combination

Example:

- Infinite Craft

Core interaction:

    A + B → C

Difference from AI Craypas:

AI Craypas is not primarily about combining two concepts into a new concept.

It explores a pathway:

    A → intermediate concepts → B

---

### 2. Knowledge Navigation

Examples:

- Six Degrees of Wikipedia
- Wikipedia speedrun formats
- Knowledge graph exploration tools

Core interaction:

Find a shortest route through an existing graph.

Difference from AI Craypas:

AI Craypas does not prioritize shortest distance.

It prioritizes an understandable and unexpected pathway.

---

### 3. Human Pathfinding Games

Examples:

- Word association games
- Word ladder formats
- Wiki Game
- NYT Connections
- Only Connect

Core interaction:

The user actively finds or guesses the connection.

Difference from AI Craypas:

AI Craypas initially focuses on AI-generated pathways that users can inspect, compare, react to, and save.

Future versions may introduce prediction or comparison mechanics.

---

### 4. Curated Interdisciplinary Chains

Examples:

- James Burke's Connections
- Educational essays
- Curated “today I learned” content
- Interdisciplinary documentary formats

Core interaction:

A human curator connects distant topics through historical, scientific, or cultural chains.

Difference from AI Craypas:

AI Craypas aims to generate a pathway on demand from user-selected concepts.

---

### 5. Computational Creativity

Related areas:

- Metaphor generation
- Conceptual blending
- Associative reasoning
- Creative ideation tools

Difference from AI Craypas:

Most related systems focus on metaphor generation, semantic similarity, or idea recombination.

AI Craypas focuses on an explainable multi-hop route between two fixed endpoints.

---

## Current Hypothesis

A widely known mainstream consumer product focused on:

> user-selected concepts  
> → explainable multi-hop pathway  
> → fact / analogy distinction  
> → structured surprise  
> → saveable personal sketchbook

has not yet been clearly identified.

This is not a claim that no similar project exists.

It is a working research hypothesis that requires continued validation through product research, web search, and model experimentation.

---

## Product Risks

### Hallucination Risk

LLMs may create pathways that sound convincing but contain inaccurate facts.

Possible mitigation:

- Ground factual claims with search or source retrieval
- Mark claims that require verification
- Separate factual links from analogical links
- Allow users to inspect sources later

### Arbitrary Connection Risk

A path can feel clever but still be logically weak.

Possible mitigation:

- Require a reason for every hop
- Reject abrupt semantic jumps
- Use structured output rules
- Compare multiple candidate pathways internally
- Let users mark paths as strong, weak, surprising, or unclear

### Passive Consumption Risk

A user may only enter two words, read the result, and leave.

Possible mitigation:

- Hide one or more intermediate nodes
- Let users predict the next hop
- Let users compare multiple pathways
- Let users save and annotate discoveries
- Offer a daily random concept pair
