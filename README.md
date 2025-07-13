# Prompt Engineering Repo

## Overview

This repository collects various prompt engineering templates for LLMs. Prompts are categorized (archived, current, in-progress) with raw files in `prompts/`. Detailed explanations live in `docs/`. Assets (e.g., images) are in `assets/`.

Focus: General-use, analysis, reasoning, and coding prompts. Contributions welcome!

## Repo Structure

- **assets/**: Images and visuals (e.g., diagrams).
- **docs/**: Explanations and guides (e.g., when to use prompts).
- **prompts/**:
  - **archived/**: Older or deprecated prompts (e.g., AI tutor variants).
  - **current/**: Active, ready-to-use prompts (e.g., general.md).
  - **in-progress/**: Drafts/experiments (e.g., vanilla coding variants).

## Available Prompts

### Current Prompts

- [hqrn_v1.0.md](prompts/current/reasoning/hqrn_v1.0.md): HoloFractal Quantum Reasoning Nexus (creative/exploratory).
- [vanilla_reasoning_v2.3.md](prompts/current/reasoning/vanilla_reasoning_v2.3.md): 8-step cycle for rigorous reasoning.
- [vanilla_coding_v2.0.md](prompts/current/coding/vanilla_coding_v2.0.md): Structured coding framework with Git/TDD.
- [vanilla_coding_v1.4.md](prompts/current/coding/vanilla_coding_v1.4.md): Experimental coding variant with context-gathering loop "bug/feature".
- [prompt_analysis.md](prompts/current/prompt_analysis.md): Analyzes other prompts for improvements.

### In-Progress Prompts

- [vanilla-coding-v1.4.md](prompts/in-progress/vanilla-coding-v1.4.md): Experimental coding variant with context-gathering loop "bug/feature".

### Documentation

- [reasoning-frameworks.md](docs/reasoning-frameworks.md): Details on various reasoning prompts, such as HQRN and Cognitive Cycle (Vanilla Reasoning prompts).
- [coding-frameworks.md](docs/coding-frameworks.md): Details on various coding prompts, such as Vanilla Coding variants (including v1.4 bug doc).

## Getting Started

1. Copy a prompt from `prompts/` into your LLM interface (e.g., as system prompt).
2. Read docs for guidance on when/how to use.
3. For development: Clone repo, add new prompts to `prompts/in-progress/`, then move to current when ready.

## Contributing

- Add new prompts via PR to `prompts/in-progress/`.
- Suggest docs updates for explanations.
- Follow structure for consistency.

Last updated: July 13, 2025