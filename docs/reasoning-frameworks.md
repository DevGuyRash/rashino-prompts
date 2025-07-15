# Reasoning Frameworks Prompts

## Overview

This document explains two advanced reasoning framework prompts: **HQRN (HoloFractal Quantum Reasoning Nexus)** and **Cognitive Cycle**. These are designed for structured, high-quality LLM outputs. Based on testing, here's what they're good for, when to use them, and model considerations.

### HQRN (HoloFractal Quantum Reasoning Nexus)

- **What It's Good At**: Creative exploration, hypothesis generation, and parallel idea evolution. Uses metaphors (quantum superposition, fractals) for novelty-excels in brainstorming, story outlines, or multi-perspective analysis.
- **When to Use**:
  - Creative tasks (e.g., idea generation, fiction outlines).
  - Exploratory queries needing multiple "realities" (e.g., scenario planning).
  - On high-quality reasoning models (e.g., Grok 4, o3) for enhanced flair; on non-reasoning models for added structure.
  - Avoid for pure facts (too abstract) or low-quality models (risks incoherence).
- **Example Usage**: Paste as system prompt for tasks like "Generate a story based on fractals."

Raw prompt file: [../prompts/current/reasoning/hqrn_v1.0.md](../prompts/current/reasoning/hqrn_v1.0.md)

### Cognitive Cycle

- **What It's Good At**: Rigorous, verifiable reasoning with tools/recursion. Strong for fact-heavy research, planning, or debugging-includes adversarial critiques for robustness. The v2.3.3 update includes enhanced neurosymbolic enforcement and refined error containment protocols for even greater reliability and precision.
- **When to Use**:
  - Complex analytical tasks (e.g., research, multi-step planning).
  - When verification/tools are key (e.g., on reasoning models like o3 for deep iteration).
  - On low-quality models to enforce structure; on high-quality non-reasoning for added logic.
  - Avoid for simple creativity (too verbose/rigid).
- **Example Usage**: Use for queries like "Plan a virtual conference with critiques."

Raw prompt file: [../prompts/current/reasoning/vanilla_reasoning_v2.3.3.md](../prompts/current/reasoning/vanilla_reasoning_v2.3.3.md)

### Comparisons and General Tips

- **HQRN vs. Cognitive Cycle**: HQRN for creativity/novelty (lighter, metaphorical); Cognitive for depth/rigor (recursive, tool-focused). Use HQRN for ideation, Cognitive for execution.
- **Model Considerations**:
  - **High-Quality Reasoning (e.g., o3, Grok 4)**: Both enhance; HQRN adds flair, Cognitive leverages built-ins.
  - **Low-Quality Reasoning**: Cognitive to add structure; avoid HQRN (too abstract).
  - **High-Quality Non-Reasoning**: HQRN for creativity; Cognitive for analysis.
  - **Low-Quality Non-Reasoning**: Neither-stick to vanilla or simpler prompts.
- **Tips**: Test on sample tasks; combine for hybrids (e.g., HQRN for ideas, then Cognitive for refinement). Link raw files in README for easy copy-paste.

For more, see [README.md](../../README.md).