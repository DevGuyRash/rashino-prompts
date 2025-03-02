# Prompt Analysis

## Overview

These prompts are meant to be used to analyze other prompts. Whether the end-goal is improvement, debugging, or deconstruction, these prompts are designed to help.

## Prompts

### Prompt Framework Mapping

This prompt is meant to identify known methodologies, frameworks, and concepts that are being recreated in the text and wasting tokens and technical precision.

It's essentially discovering the `unknown unknown` concepts that the author is unaware of.

For example, someone may say, "I want you to use bullet points with a left bracket, space, and right bracket. Then the text will follow and you will do this for the rest of the response." It would be more accurate to say, "I want you to respond using markdown task lists." If the author does not know of the concept of markdown task lists, they will likely have to write a lot more text to accomplish the same task.

To use this prompt, replace `[TEXT FOR ANALYSIS]` with the text you want to analyze.

`````md
Act as an expert research professor performing Prompt Ontology Mapping using git merge-conflict visualization.

Analyze a given prompt to identify areas where the author unintentionally "reinvents the wheel," recreating established methodologies, frameworks, concepts, or techniques instead of explicitly referencing them.

Use Donald Rumsfeld's known-knowns framework explicitly:

- Known Knowns: Explicitly named frameworks.
- Known Unknowns: Structured sections resembling known frameworks but uncertain in precise identification.
- Unknown Unknowns: Sections unintentionally recreating established frameworks without explicitly naming them (primary target).

Your Task:

1. Segment the provided prompt into logical sections (instructions, tasks, outputs, methods, or subsections).

2. For each section, identify clearly and precisely the unknown unknowns:
   - Methodologies/Frameworks Identified (with Original Domains):
     - Precisely bullet-list each identified methodology/framework alongside its domain (e.g., Eisenhower Matrix: Time Management).
   - Original Domain(s):
     - Specify domains or disciplines of identified methodologies/frameworks.
   - Specific Technical Elements Recreated:
     - Bullet-list technical elements indicating recreation (only include elements clearly reinventing established frameworks/concepts).
   - Recreated Concepts or Techniques (if applicable):
     - List broader concepts or techniques recreated.

3. Optimization Recommendations:
   - Provide succinct ways to explicitly reference identified methodologies/frameworks, avoiding verbose explanations. Offer multiple alternatives if helpful.

4. Fully Optimized Final Prompt:
   - Provide a fully optimized rewrite explicitly using the identified methodologies/frameworks clearly and succinctly.

Required Annotation Format (exactly):

````md
<<<<<<< ORIGINAL TEXT
[exact original text segment]
=======
- Methodologies/Frameworks Identified:
  - Framework/Methodology 1: [domain]
  - ...
  - Framework/Methodology N: [domain] (if applicable)

- Specific Technical Elements Recreated:
  - Technical element 1
  - ...
  - Technical element N (if applicable)

- Recreated Concepts or Techniques (if applicable):
  - Concept/Technique 1
  - ...
  - Concept/Technique N (if applicable)

- Optimization Recommendations:
  - Recommendation 1
  - ...
  - Recommendation N (if applicable)

- Fully Optimized Final Prompt:
  > [Fully optimized rewritten prompt explicitly referencing frameworks/methodologies]
>>>>>>> ANNOTATION
````

... (continue for each section)

**Final Prompt:**

````md
[Final optimized prompt combining all improved annotations]
````

Example Annotations:

````md
<<<<<<< ORIGINAL TEXT
When managing tasks, categorize them by urgency and importance. Some require immediate attention, while others are important but can be scheduled for later. Tasks that are urgent but less critical can be delegated, and tasks neither urgent nor important should be eliminated.
=======
- Methodologies/Frameworks Identified:
  - Eisenhower Matrix: Time Management

- Specific Technical Elements Recreated:
  - Four-category task prioritization matrix (urgent/important)

- Optimization Recommendations:
  - Explicitly instruct to use the "Eisenhower Matrix."

- Fully Optimized Final Prompt:
  > Use the Eisenhower Matrix to prioritize tasks effectively.
>>>>>>> ANNOTATION
````

````md
<<<<<<< ORIGINAL TEXT
Clearly define what you're trying to accomplish. Ensure your goals are trackable, achievable within your capabilities, realistically attainable, and bound by a timeframe.
=======
- Methodologies/Frameworks Identified:
  - SMART Goal Framework: Project Management

- Specific Technical Elements Recreated:
  - Goal criteria: specific, measurable, achievable, realistic, time-bound

- Optimization Recommendations:
  - Explicitly instruct to set goals using the "SMART Goal Framework."

- Fully Optimized Final Prompt:
  > Clearly set goals following the SMART Goal Framework.
>>>>>>> ANNOTATION
````

````md
<<<<<<< ORIGINAL TEXT
When solving problems, first observe and clearly define the issue. Propose potential explanations or solutions. Systematically test each proposal, evaluate outcomes, and adjust your understanding based on results.
=======
- Methodologies/Frameworks Identified:
  - Scientific Method: Science/Research Methodology

- Specific Technical Elements Recreated:
  - Observation, hypothesis, experimentation, evaluation, and refinement cycle

- Optimization Recommendations:
  - Explicitly instruct to use the "Scientific Method."

- Fully Optimized Final Prompt:
  > Solve problems systematically using the Scientific Method.
>>>>>>> ANNOTATION
````

**Final Prompt:**

````md
[Final optimized prompt combining all improved annotations]
````

Prioritize accuracy, specificity, and clarity in your annotations.

Now analyze the following text:

~~~
[TEXT FOR ANALYSIS]
~~~
`````

#### Example Outcomes

- [ChatGPT - Framework Reinvention Analysis](https://chatgpt.com/share/67c4b736-ce5c-8006-8d2f-e95404a1796f)