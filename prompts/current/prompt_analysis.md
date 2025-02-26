# Prompt Analysis

## Overview

These prompts are meant to be used to analyze other prompts. Whether the end-goal is improvement, debugging, or deconstruction, these prompts are designed to help.

## Prompts

### Prompt Framework Mapping

This prompt is meant to identify known methodologies, frameworks, and concepts that are being recreated in the text and wasting tokens and technical precision.

It's essentially discovering the `unknown unknown` concepts that the author is unaware of.

For example, someone may say, "I want you to use bullet points with a left bracket, space, and right bracket. Then the text will follow and you will do this for the rest of the response." It would be more accurate to say, "I want you to respond using markdown task lists." If the author does not know of the concept of markdown task lists, they will likely have to write a lot more text to accomplish the same task.

`````md
Act as a research professor performing prompt ontology mapping using git merge conflict visualization. 

Think in terms of the Johari Window Framework. The text below is likely a "blind spot" for the author and many known concepts are being recreated due to the `unknown unknown` quadrant.

The goal is to identify such sections of the text that are recreating established methodologies/frameworks/concepts and to annotate them; thus, eliminating any verbose attempts to "reinvent the wheel".

Break the text into logical sections, and for each section, identify all likely `unknown unknown` concepts that are being recreated. Identify specific established methodologies being recreated in this text, using the most precise technical terminology possible. For each section:

1. Name exact methodologies (e.g., "Work Breakdown Structure" not just "task breakdown")
2. Specify the original domain (e.g., "from systems engineering")  
3. Highlight specific technical elements being recreated

Use this exact format for each section (inside a quadruple backtick code block):

````
<<<<<<< ORIGINAL TEXT
[paste original text here with exact formatting]
=======
[your bullet point analytical annotation here - identify established methodologies/frameworks/concepts this text is recreating]
>>>>>>> ANNOTATION
````

Prioritize precision in identifying exact methodologies over general observations.

Analyze this text:

~~~
[TEXT FOR ANALYSIS]
~~~
`````