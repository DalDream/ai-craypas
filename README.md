# AI Craypas

> There are no unrelated concepts — only undiscovered pathways.

## Core Question

**Can AI make humans more creative?**

Generative AI is often used to produce finished outputs on behalf of people.

AI Craypas explores a different role for AI: not replacing human creation, but revealing unexpected and understandable connections that may help people think, imagine, and create something new.

> There are no unrelated concepts — only undiscovered pathways.

AI Craypas is an exploratory concept for generating understandable, multi-hop pathways between two seemingly unrelated concepts.

It does not try to find the shortest route, the most similar word, or a single correct answer.

Instead, it asks:

> What hidden path can connect these two ideas?

---

## The Interaction

AI Craypas is an exploratory concept for generating understandable, multi-hop pathways between two seemingly unrelated concepts.

It does not try to find the shortest route, the most similar word, or a single correct answer.

Instead, it asks:

> What hidden path can connect these two ideas?

---

## The Interaction

Most existing concept tools focus on one of the following:

- Combining concepts: `A + B → C`
- Finding the shortest path between existing knowledge nodes
- Retrieving semantically similar concepts
- Letting users manually discover links through games or browsing

AI Craypas explores a different interaction:

    User chooses two concepts
    ↓
    AI generates a multi-hop conceptual pathway
    ↓
    Each hop explains why the connection exists
    ↓
    The user explores, evaluates, and saves discoveries

The goal is not answer-finding.

The goal is **structured surprise**.

---

## Core Principles

### Every hop should be understandable

A pathway should not jump between unrelated words without explanation. Each connection should include a short reason explaining why the next concept follows from the previous one.

### Facts and analogies must be distinguished

Not every meaningful connection is factual. AI Craypas should distinguish between:

- **Fact** — a verifiable scientific, historical, geographic, linguistic, or cultural relationship
- **Structural Analogy** — a shared mechanism, form, process, or pattern
- **Cultural Connection** — a relationship through art, media, language, mythology, or collective references

### Surprise is not enough

A path should be unexpected, but it should remain legible.

> I would not have connected these before, but now I understand why.

### Multiple pathways can coexist

The same two concepts may be connected through entirely different domains: scientific, historical, cultural, or structural.

The existence of multiple understandable routes is part of the experience.

---

## Prototype Scope

### Input

Two concepts selected by the user.

Example: `Fingernail → Magellan`

### Output

- A pathway of 4–6 nodes
- A one-line explanation for every hop
- Connection-type tags
- A short discovery insight
- Optional save to a personal sketchbook

Example output shape:

    Start concept
    → Intermediate concept [Fact]
    → Intermediate concept [Structural Analogy]
    → End concept

    Discovery:
    A short insight revealed by following the pathway.

---

## Product Hypothesis

Large language models may be useful not only for answering questions, but also for surfacing understandable pathways between distant concepts across science, history, culture, geography, language, and art.

AI Craypas tests whether this capability can become a playful and useful discovery experience.

Potential use cases include:

- Creative brainstorming
- Writing and worldbuilding
- Educational discovery
- Curiosity-driven exploration
- Short-form knowledge content
- Personal idea sketchbooks

---

## Current Status

**Idea exploration / pre-prototype**

This repository documents the concept, early examples, adjacent references, and validation questions.

The next step is to test the same concept pairs across multiple models using identical prompts and evaluation criteria.
