# RPAC: The Unified Theory of Recursive Memory

A Bio-Mimetic, Model-Agnostic, Multi-Layered Memory Architecture for Persistent LLM Agents.

---

## Overview

Current LLM architectures suffer from a critical flaw: **they treat context as a flat, volatile buffer.** This leads directly to "Context Bloat" (exponential cost growth), "IQ-Starvation" (loss of immediate reasoning power), and "Identity Drift" (the gradual erosion of the agent's core directives over long sessions).

**RPAC (Recursive Paced Abstract Context)** resolves the fundamental tension between context-window physics, economic sustainability, and agentic stability. Inspired by human cognitive structures—the interplay between working memory, the hippocampus, and the cerebral cortex—RPAC externalizes a structured memory consolidation process onto the LLM. 

By separating **what the agent is** (Identity) from **what the agent has done** (Experience), RPAC turns the LLM from a simple text-predictor into a structured, sustainable cognitive engine. 

**The future of AI is not in the capacity of the buffer, but in the elegance of the architecture that manages it. RPAC Is All We Need.**

---

## I. The Three-Layered Cognitive Architecture
[ PAC: The Constitutional Core ] <--- Immutable Anchor (Identity)
|
[ NC: Non-Compressed Workspace ] <--- 2k~4k Tokens (Current Task IQ)
|
v (Context Saturation Trigger)
[ RAC Layer 1: Raw Summary     ] <--- Mid-Size
|
v (Recursive Filtering)
[ RAC Layer 2: High Abstraction] <--- Small-Size (Noise Purged)
|
~~<--- The number of layers can be set freely
|
v (Final Consolidation)
[ RAC Top Layer: Global Wisdom ] <--- Large Size (Pure History)

### 1. PAC (Primary & Absolute: The Constitutional Core)
* **Role:** Enforces behavioral constraints, long-term mission objectives, and the agent's fundamental persona.
* **Property:** Completely immune to runtime modification, compression, or eviction. 
* **Impact:** De-couples system prompts from mutable dialogue history, eliminating "Identity Drift."

### 2. NC (Now Context / Non-compressed: The Working Memory)
* **Role:** The high-fidelity front line of execution. This is the agent's active desk where debugging, complex logic parsing, and precise prompt interactions take place.
* **Property:** Raw text, zero compression, high-frequency access.
* **Sanctuary Rule:** To prevent "IQ-starvation," $T_{NC}$ must maintain a strict reservation of **2,000 to 4,000 tokens**. Shrinking this pool destroys the agent's immediate operational intelligence.

### 3. RAC (Recent Abstract Context / Recursive Stratification: The Tiered Memory)
* **Role:** The experience archivist. As conversations age, they move through successive layers of recursive compression.
* **Time-Gradient Dynamic:** * **Large Layer Sizes:** Slows down time-travel; keeps conversational details alive longer.
  * **Small Layer Sizes:** Accelerates time; turns raw text into highly dense conceptual summaries almost instantly.
* **The Result:** The agent can reference a pivotal decision made weeks ago without spending a million tokens of raw, redundant chat logs.

---

## II. Recursive Trigger & Consolidation Dynamics

To guarantee deterministic resource management, each layer ($L$) is bound by an explicit, pre-defined maximum token capacity ($C_{max}$). Compression and vertical stratification are strictly triggered just before breaching these hard ceilings.

### 1. NC to RAC Layer 1 Eviction
When the token count of the active workspace ($T_{NC}$) approaches its physical ceiling, the oldest conversation blocks are compressed into semantic summaries:
$$\text{If } T_{NC} \ge C_{max}(NC) - \epsilon$$
*(Where $\epsilon$ represents a minimal safety buffer allocation).*

### 2. Recursive Cascade Between RAC Layers
Each successive RAC layer ($L_n$) operates under identical hard-ceiling mechanics. When a layer saturates, it filters out historical noise and pushes highly abstract concepts to the next tier:
$$\text{If } T_{L_n} \ge C_{max}(L_n) - \epsilon$$

### 3. Top-Layer Deep Redistillation (Global Wisdom)
The highest layer, **RAC Top Layer**, is also governed by a strict physical limit to prevent infinite expansion. 
$$\text{If } T_{\text{Top}} \ge C_{max}(\text{Top}) - \epsilon$$
Upon reaching this threshold, the layer undergoes **Deep Redistillation**, shifting from chronological history to immutable, high-dimensional axioms (the agent's personal philosophy and core historical lessons). This enforces a definitive **Hard Ceiling Rule**, ensuring the agent's total memory footprint never overloads the system, regardless of session longevity.

---

## III. Agentic Autonomy & Identity Isolation

In traditional frameworks, autonomous agents fail over long iterations because the accumulation of raw execution loops and error logs contaminates the context window. The agent literally "forgets" what it was built to do.

RPAC solves this via **Identity Isolation**. Because the **PAC** remains unpolluted by the operational data flowing into **NC** and condensing into **RAC**, an agent can spawn infinite sub-tasks, process thousands of environmental feedback loops, and self-correct endlessly while remaining perfectly anchored to its original mandate. 

---

## IV. Hardware Scaling & The Hard Ceiling Rule

RPAC adapts dynamically to the underlying compute limits of both edge hardware and frontier cloud models:

* **Local / Edge Optimization (<10B Parameters):** This prevents Out-Of-Memory (OOM) errors and allows small models to punch far above their weight in long-term task retention.
* **Frontier Cloud Optimization (e.g., Gemini 1.5 Pro):** It builds a flawless "God-Mode Long-Term Memory" that structurally indexes chronological events across massive physical boundaries.

---

## V. The Economic and Ecological Mandate

1. **Direct Cost Reduction:** Compressing historical context into semantic layers slashes the total token count of every recursive API request, driving operational overhead down by an order of magnitude.
2. **Energy Efficiency ("Green AI"):** Processing optimized, compressed context streams drops the required FLOPS per inference cycle, drastically reducing the carbon and compute load on modern data centers.

---

## License

This architecture is open-source and distributed under the **Apache 2.0 License**. 

*Under the Apache 2.0 framework, you are free to use, modify, and distribute this architecture for both personal and commercial applications. However, any contributor or user attempting to leverage patent litigation against the maintainers or users of this project regarding its core design will face immediate, automatic termination of their usage rights.*

![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)
