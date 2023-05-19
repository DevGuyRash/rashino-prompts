# Table of Contents

<!-- TOC -->
* [Table of Contents](#table-of-contents)
* [Prompt Information](#prompt-information)
  * [Prompt Structure](#prompt-structure)
    * [Prompt Template](#prompt-template)
  * [Mandatory Control Tokens](#mandatory-control-tokens)
* [Control Token Options](#control-token-options)
  * [Control Token Lists](#control-token-lists)
* [Prompt Generators](#prompt-generators)
  * [Prompt Creator](#prompt-creator)
<!-- TOC -->

# Prompt Information

The point of this structure is to extract the common essentials behind most prompt frameworks:

- **The system message** to control the context (and sometimes restrictions)
- **The user instructions** for telling the LLM what to do
- **The control tokens** often weaved into the prompt itself or manipulated in some other way, such as the formatting,
  restrictions, persona, etc.
- **The keywords** which are the focal point of the output
- **Example output** which demonstrates how a finished output should look

The goal of this idea is to standardize prompts that are meant for everyday use so that a person will not need to
memorize very complex frameworks or prompts in order to get great results, instead they can just fill in the sections
and _optionally_ convert it to natural language to be used again later.

## Prompt Structure

**System Message:** (User text)

**Instructions:** (User text)

**Control Tokens**

* **[Persona]** option
* **[Objective]** option
* **[Target Audience]** option
* **[Output Format]** option
* **[Emotional Tone]** option
* **[Formality Level]** option
* **[Writing Style]** option
* **[Constraints]** option
  * **[Token]** Option
  * **[Token]** Option
  * Etc.
* **[Additional relevant control tokens]** Option

**Keywords:** (User text)

**Example Output:**

~~~
Example output
~~~

### Prompt Template

**System Message:** Use this template to craft unique and detailed prompts for a large language model. Remember to
specify your requirements accurately and choose control tokens and keywords that are most relevant to your desired
output.

**Instructions:** Please fill in the template below, following the guidelines provided. Ensure to select appropriate
options for each control token and provide relevant keywords to guide the generation of the output. You can add more
control tokens and sections if necessary, but aim for a balance between specificity and flexibility to get the most
optimal results.

**Control Tokens**

* **\[Objective\]** Choose from: Inform, Entertain, Persuade, Educate
* **\[Target Audience\]** Choose from: General Public, Children, Adults, Subject Matter Experts
* **\[Output Format\]** Choose from: Fictional Narrative, Factual Narrative, Technical Details, Email Format, Essay
  Format, Dialogue Format, Q&A Format
* **\[Emotional Tone\]** Choose from: Serious, Humorous, Formal, Informal, Authoritative, Friendly, Optimistic,
  Pessimistic, Playful, Sarcastic
* **\[Formality Level\]** Choose from: Formal, Informal
* **\[Language\]** Choose from: English, Spanish, French, German (or any other language you prefer)
* **\[Output Length\]** Choose from: Short, Medium, Long
* **\[Persona\]** Choose from: Historian, Scientist, Fiction Writer, Journalist, Educator, Critic, Advisor, Debater
* **\[Writing Style\]** Choose from: Academic, Analytical, Argumentative, Conversational, Creative, Critical,
  Descriptive, Expository, Informative, Narrative, Persuasive
* **\[Additional Token\]** Option - Add more control tokens from the provided list or based on your needs. Be sure to
  specify the desired option.

**Keywords:** \[Provide the main keywords related to the topic or theme of your content\]

**Example Output:**

```
[Provide a brief sample of the type of content you would like to generate. This could include specific phrases, sentences, or a general outline of the desired structure and content.]
```

## Mandatory Control Tokens

* Persona
* Objective
* Target Audience
* Output Format
* Emotional Tone
* Formality Level
* Writing Style
* Constraints

# Control Token Options

These are the possible control tokens. Please feel free to expand the list, sections, etc.

- It is important not to utilize too many, or too restricting ones, as it takes away from the ability to produce diverse
  output.

## Control Token Lists

- [With Descriptions](token_options.md)
- [Without Descriptions](token_options_without_desc.md)
- [Without Formatting](token_options_without_any.md)

# Prompt Generators

## Prompt Creator

Your task is to craft a specialized prompt with the purpose of [PURPOSE]. The prompt should be optimized for a natural language processing large language model in a format like the example output. Choose the appropriate control tokens and relevant keywords, filling in the template below.

You can add either more sections or more control tokens per section if you think they are necessary. Having multiple control tokens per section is fine but try to use only one or two per section.

Mandatory control tokens:

* Persona
* Objective
* Target Audience
* Output Format
* Emotional Tone
* Formality Level
* Writing Style
* Constraints

List of control tokens:

1. Objective
    * Inform
    * Entertain
    * Persuade
    * Educate
2. Target Audience
    * General Public
    * Children
    * Adults
    * Subject-Matter Experts
3. Output Format
    * Fictional Narrative
    * Factual Narrative
    * Technical Details
    * Email Format
    * Essay Format
    * Dialogue Format
    * Q&A Format
4. Writing Style
    * Academic
    * Analytical
    * Argumentative
    * Conversational
    * Creative
    * Critical
    * Descriptive
    * Expository
    * Informative
    * Narrative
    * Persuasive
5. Emotional Tone
    * Serious
    * Humorous
    * Formal
    * Informal
    * Authoritative
    * Friendly
    * Optimistic
    * Pessimistic
    * Playful
    * Sarcastic
6. Formality Level
    * Formal
    * Informal
7. Narrative Perspective
    * First Person
    * Second Person
    * Third Person
8. Genre
    * Science Fiction
    * Fantasy
    * Mystery
    * Romance
9. Persona
    * Historian
    * Scientist
    * Fiction Writer
    * Journalist
    * Educator
    * Critic
    * Advisor
    * Debater
10. Language Preference
    * English
    * Spanish
    * French
    * German
11. Complexity Level
    * Simple
    * Intermediate
    * Advanced
12. Structure
    * Linear
    * Non-linear
13. Argument Stance
    * Pro
    * Con
    * Balanced
14. Setting
    * Personal
    * Professional
    * Academic
    * Social
    * Historical
    * Futuristic
    * Realistic
    * Fantastical
    * Scientific
    * Artistic
15. Document Format
    * Essay
    * Report
    * Letter
    * Blog Post
    * Tweet
    * Script
    * News Article
    * Review
    * Short Story
    * Poem
    * Dialogue
    * Q&A
    * Bullet Points
    * Listicle
16. Constraints
    * Word Count Limit
    * Time Period
    * Specific Themes
    * Specific Characters
    * Specific Settings
    * Specific Genres
    * Language Restrictions
    * Content Restrictions
17. Detail Level
    * High
    * Medium
    * Low
18. Factuality
    * Factual
    * Fictional
19. Output Length
    * Short
    * Medium
    * Long

Example output:

"""

System Message: (Text)

Instructions: (Text)

Control Tokens

* [Persona] option
* [Objective] option
* [Target Audience] option
* [Output Format] option
* [Emotional Tone] option
* [Formality Level] option
* [Writing Style] option
* [Constraints] option
  * [Token] Option
  * [Token] Option
  * etc.
* [Token] Option
    * Add tokens from the list or your own knowledge, as necessary.

Keywords: [Text]

Example Output

~~~
(Text)
~~~

"""