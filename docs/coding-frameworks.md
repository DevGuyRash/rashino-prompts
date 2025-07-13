# Coding Frameworks Prompts

## Overview

This document covers coding-specific reasoning frameworks: **Vanilla Coding v2.0** and **Vanilla Coding v1.4**. These build on neurosymbolic cycles for code tasks (e.g., Git workflows, TDD). v1.4 has a documented "bug" that's useful as a feature in agentic tools.

### Vanilla Coding v2.0

- **What It's Good At**: Structured coding with tools/recursion, Git enforcement, and TDD. Ideal for development, debugging, or planning code changes-emphasizes verification and error handling.
- **When to Use**:
  - Coding tasks (e.g., fixing bugs, building features).
  - On high-quality reasoning models (e.g., Grok 4, o3) for robust automation; on non-reasoning for added logic.
  - Avoid for non-code creativity (too prescriptive).
- **Example Usage**: System prompt for "Implement a feature with tests."

Raw prompt file: [../prompts/current/coding/vanilla_coding_v2.0.md](../prompts/current/coding/vanilla_coding_v2.0.md)

### Vanilla Coding v1.4

- **What It's Good At**: Similar to v2.0 but with a unique bug causing near-infinite context gathering in Part B (resets to State after partial harvesting, asking evolving questions). This "bug" acts as a feature in agentic tools (e.g., Cursor, Gemini CLI, Claude Code) for exhaustive exploration-gathers deep context before acting, useful for complex debugging or research-heavy code.
- **Bug Documentation**: The loop stems from incomplete harvesting (resets after one question, rephrasing others). It eventually progresses but prioritizes context. Per tests/searches, similar loops in agents (e.g., Cursor infinite commands) can enable thoroughness if managed-use in tools supporting interruptions.
- **When to Use**:
  - Agentic coding where deep context is key (e.g., large projects in Cursor).
  - On reasoning models for iterative depth; avoid on low-quality (exacerbates loops).
  - Never for quick tasks (loop delays).
- **Example Usage**: In Cursor for "Debug a repo"-lets it gather extensively.

Raw prompt file: [../prompts/current/coding/vanilla_coding_v1.4.md](../prompts/current/coding/vanilla_coding_v1.4.md)

### Comparisons and Tips

- **v2.0 vs. v1.4**: v2.0 for stable, efficient coding; v1.4 for exploratory/agentic with its "infinite" gathering as a feature.
- **Model Considerations**:
  - **High-Quality Reasoning**: Both strong; both leverage loops for depth, but v1.4 has a bug that can be useful in agentic tools.
  - **Low-Quality Reasoning**: v2.0 to enforce structure; avoid v1.4 (uncontrolled loops).
  - **High-Quality Non-Reasoning**: v2.0 for basics; v1.4 risky.
  - **Low-Quality Non-Reasoning**: Neither-use vanilla.
- **Tips**: Monitor v1.4 loops in agents; interrupt if needed. Test for your workflow.

For more, see [README.md](../../README.md).