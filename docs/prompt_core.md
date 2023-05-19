# Table of Contents

<!-- TOC -->

* [Table of Contents](#table-of-contents)
* [Prompt Information](#prompt-information)
    * [Prompt Structure](#prompt-structure)
        * [Prompt Template](#prompt-template)
    * [Mandatory Control Tokens](#mandatory-control-tokens)
* [Control Token Options](#control-token-options)
* [With Descriptions](#with-descriptions)
    * [Without Descriptions](#without-descriptions)
    * [Without Options or Formatting](#without-options-or-formatting)
* [Prompt Generators](#prompt-generators)
    * [Create Prompt](#create-prompt)

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

- **[Purpose]** Option
- **[Audience]** Option
- **[Content Type]** Option
- **[Tone]** Option
- **[Formality]** Option
- **[Language]** Option
- **[Length]** Option
- **[Role]** Option
- **[Writing Approach]** Option
- **[Additional relevant control tokens]** Option

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

* Objective
* Target Audience
* Output Format
* Emotional Tone
* Formality Level
* Language
* Output Length
* Persona
* Writing Style

# Control Token Options

These are the possible control tokens. Please feel free to expand the list, sections, etc.

- It is important not to utilize too many, or too restricting ones, as it takes away from the ability to produce diverse
  output.

# With Descriptions

1. <u>**Objective** _(Specify the purpose or goal of the text)_</u>

    * **Inform** (The output will focus on providing factual information, explanations, or instructions.)
    * **Entertain** (The output will prioritize creating an enjoyable or engaging narrative.)
    * **Persuade** (The output will aim to convince or influence the reader's opinions or actions.)
    * **Educate** (The output will emphasize teaching or enlightening the reader about a particular topic.)
2. <u>**Target Audience** _(Specify the intended audience for the text)_</u>

    * **General Public** (The output will be suitable for a wide range of readers without specific expertise.)
    * **Children** (The output will be tailored for young readers, considering their age, understanding, and
      appropriateness.)
    * **Adults** (The output will cater to a mature audience, assuming a certain level of knowledge and comprehension.)
    * **Subject Matter Experts** (The output will be directed towards professionals or individuals with specialized
      knowledge in a particular field.)
3. <u>**Output Format** _(Specify the desired format or structure of the output)_</u>

    * **Fictional Narrative** (The output will be presented as a creative story or fictional account.)
    * **Factual Narrative** (The output will provide information in a narrative form, combining facts and storytelling
      elements.)
    * **Technical Details** (The output will focus on providing precise technical information or specifications.)
    * **Email Format** (The output will be structured like an email, suitable for communication purposes.)
    * **Essay Format** (The output will follow the structure of an essay, including an introduction, body paragraphs,
      and conclusion.)
    * **Dialogue Format** (The output will be formatted as a conversation or dialogue between two or more speakers.)
    * **Q&A Format** (The output will be organized as a question-and-answer format, providing responses to specific
      queries.)
4. <u>**Writing Style** _(Specify the desired style or tone of the writing)_</u>

    * **Academic** (The output will adhere to formal academic writing conventions, including citations and references.)
    * **Analytical** (The output will involve critical analysis and examination of the subject matter.)
    * **Argumentative** (The output will present a clear argument or position on a topic, supporting it with evidence
      and reasoning.)
    * **Conversational** (The output will adopt an informal and casual tone, resembling everyday conversations.)
    * **Creative** (The output will prioritize imaginative and original expression, focusing on artistic or literary
      aspects.)
    * **Critical** (The output will involve a thorough evaluation and critique of a subject, highlighting strengths and
      weaknesses.)
    * **Descriptive** (The output will provide vivid and detailed descriptions of people, places, or events.)
    * **Expository** (The output will aim to explain or clarify a subject, providing information in a clear and concise
      manner.)
    * **Informative** (The output will focus on delivering useful and educational content, emphasizing clarity and
      accuracy.)
    * **Narrative** (The output will tell a story or recount events, emphasizing storytelling techniques.)
    * **Persuasive** (The output will employ persuasive language and rhetoric to convince the reader of a particular
      viewpoint.)
5. <u>**Emotional Tone** _(Specify the desired emotional tone conveyed in the output)_</u>

    * **Serious** (The output will convey a somber or grave tone, addressing weighty or important subjects.)
    * **Humorous** (The output will incorporate humor, wit, or comedic elements to entertain the reader.)
    * **Formal** (The output will maintain a polished and professional tone, suitable for formal contexts.)
    * **Informal** (The output will adopt a relaxed and friendly tone, resembling casual or informal conversations.)
    * **Authoritative** (The output will have a commanding and confident tone, asserting expertise or credibility.)
    * **Friendly** (The output will convey warmth and approachability, establishing a friendly rapport with the reader.)
    * **Optimistic** (The output will have a positive and hopeful tone, focusing on positive aspects or outcomes.)
    * **Pessimistic** (The output will have a negative or pessimistic tone, emphasizing potential drawbacks or
      problems.)
    * **Playful** (The output will have a lighthearted and playful tone, evoking a sense of fun or amusement.)
    * **Sarcastic** (The output will employ irony and sarcasm to express mockery or derision.)
6. <u>**Formality Level** _(Specify the desired level of formality in the output)_</u>

    * **Formal** (The output will adhere to formal language conventions, suitable for professional or official
      contexts.)
    * **Informal** (The output will utilize casual and relaxed language, suitable for everyday conversations.)
7. <u>**Narrative Perspective** _(Specify the desired point of view in the narrative)_</u>

    * **First Person** (The output will be written from the perspective of the narrator or a character using "I" or "
      we".)
    * **Second Person** (The output will address the reader directly, using "you" to create a sense of involvement.)
    * **Third Person** (The output will use "he," "she," "they," etc., to narrate events from an external perspective.)
8. <u>**Genre** _(Specify the desired genre for the output)_</u>

    * **Science Fiction** (The output will incorporate elements of science and technology in an imaginative or
      futuristic setting.)
    * **Fantasy** (The output will involve magic, mythical creatures, or supernatural elements in an imaginative
      setting.)
    * **Mystery** (The output will revolve around a puzzling event or crime, engaging the reader in solving the
      mystery.)
    * **Romance** (The output will focus on romantic relationships and emotions, emphasizing love and affection.)
9. <u>**Persona** _(Specify the desired persona or role for the writer in the output)_</u>

    * **Historian** (The output will embody the perspective and expertise of a historian, emphasizing historical
      accuracy.)
    * **Scientist** (The output will convey the viewpoint and knowledge of a scientist, emphasizing scientific
      principles and research.)
    * **Fiction Writer** (The output will reflect the creativity and storytelling techniques of a fiction writer.)
    * **Journalist** (The output will adopt the approach and style of a journalist, emphasizing factual reporting.)
    * **Educator** (The output will prioritize teaching and instructing the reader, adopting an educational
      perspective.)
    * **Critic** (The output will involve critical evaluation and analysis of a subject, providing assessments and
      judgments.)
    * **Advisor** (The output will offer guidance, suggestions, or recommendations to the reader.)
    * **Debater** (The output will present arguments and counterarguments, engaging in a persuasive or argumentative
      discourse.)
10. <u>**Language Preference** _(Specify the desired language for the output)_</u>

* **English** (The output will be generated in the English language.)
* **Spanish** (The output will be generated in the Spanish language.)
* **French** (The output will be generated in the French language.)
* **German** (The output will be generated in the German language.)

11. <u>**Complexity Level** _(Specify the desired complexity level of the output)_</u>

* **Simple** (The output will be straightforward and easily understandable, avoiding complex or technical concepts.)
* **Intermediate** (The output will involve moderate complexity, assuming some prior knowledge or understanding.)
* **Advanced** (The output will be more intricate and sophisticated, suitable for individuals with in-depth knowledge or
  expertise.)

12. <u>**Structure** _(Specify the desired structure or organization of the output)_</u>

* **Linear** (The output will follow a chronological or sequential order, presenting information in a linear
  progression.)
* **Non-linear** (The output will be organized in a non-sequential or unconventional manner, with jumps or variations in
  the narrative.)

13. <u>**Argument Stance** _(Specify the desired stance or perspective in an argumentative output)_</u>

* **Pro** (The output will argue in favor of a particular viewpoint or position.)
* **Con** (The output will argue against a particular viewpoint or position.)
* **Balanced** (The output will provide arguments from both sides of an issue, aiming for a balanced presentation.)

14. <u>**Setting** _(Specify the desired setting or context for the output)_</u>

* **Personal** (The output will focus on personal experiences, emotions, or perspectives.)
* **Professional** (The output will be geared towards work-related or business contexts.)
* **Academic** (The output will be situated in an educational or scholarly environment.)
* **Social** (The output will revolve around social interactions, relationships, or societal issues.)
* **Historical** (The output will be set in a historical period or context.)
* **Futuristic** (The output will take place in a future or speculative setting.)
* **Realistic** (The output will be grounded in real-world situations and believability.)
* **Fantastical** (The output will incorporate fantastical or imaginative elements.)
* **Scientific** (The output will be centered around scientific principles, experiments, or discoveries.)
* **Artistic** (The output will explore artistic expressions, creativity, or aesthetic principles.)

15. <u>**Document Format** _(Specify the desired format or type of document for the output)_</u>

* **Essay** (The output will follow the structure and conventions of an essay.)
* **Report** (The output will be formatted as a formal report, presenting information and findings.)
* **Letter** (The output will be structured as a letter, suitable for personal or professional correspondence.)
* **Blog Post** (The output will resemble a blog post, adopting a more informal and conversational tone.)
* **Tweet** (The output will be concise and limited to the character count of a tweet.)
* **Script** (The output will be formatted as a script for a play, movie, or other performance.)
* **News Article** (The output will be written in the style of a news article, providing current information or events.)
* **Review** (The output will involve evaluating and critiquing a subject or work.)
* **Short Story** (The output will be presented as a self-contained short story.)
* **Poem** (The output will be structured as a poem, emphasizing poetic devices and rhythm.)
* **Dialogue** (The output will be presented as a dialogue between two or more characters.)
* **Q&A** (The output will be organized in a question-and-answer format, providing responses to specific queries.)
* **Bullet Points** (The output will be presented as a list of concise bullet points.)
* **Listicle** (The output will be structured as a listicle, combining a list format with informative content.)

16. <u>**Constraints** _(Specify any constraints or limitations for the output)_</u>

* **Word Count Limit** (The output will be limited to a specific number of words.)
* **Time Period** (The output will be set within a particular historical, present, or future time period.)
* **Specific Themes** (The output will revolve around predefined themes or topics.)
* **Specific Characters** (The output will involve predefined characters with specific traits or roles.)
* **Specific Settings** (The output will take place in predefined settings or environments.)
* **Specific Genres** (The output will adhere to predetermined genres or literary styles.)
* **Language Restrictions** (The output will comply with language-specific rules or requirements.)
* **Content Restrictions** (The output will avoid specific topics or content deemed inappropriate or sensitive.)

17. <u>**Detail Level** _(Specify the desired level of detail in the output)_</u>

* **High** (The output will contain in-depth and comprehensive information, including intricate details.)
* **Medium** (The output will provide a moderate level of detail, striking a balance between conciseness and
  elaboration.)
* **Low** (The output will offer a concise and minimalistic approach, focusing on essential information.)

18. <u>**Factuality** _(Specify the desired factual accuracy of the output)_</u>

* **Factual** (The output will prioritize accuracy and reliability, providing information based on verified facts.)
* **Fictional** (The output will prioritize creativity and imagination, allowing for fictional elements and
  storytelling.)

19. <u>**Output Length** _(Specify the desired length of the output)_</u>

* **Short** (The output will be brief and concise.)
* **Medium** (The output will have a moderate length, providing sufficient information and details.)
* **Long** (The output will be extensive and comprehensive, allowing for a detailed exploration of the subject matter.)

## Without Descriptions

1. **Objective**
    * Inform
    * Entertain
    * Persuade
    * Educate
2. **Target Audience**
    * General Public
    * Children
    * Adults
    * Subject Matter Experts
3. **Output Format**
    * Fictional Narrative
    * Factual Narrative
    * Technical Details
    * Email Format
    * Essay Format
    * Dialogue Format
    * Q&A Format
4. **Writing Style**
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
5. **Emotional Tone**
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
6. **Formality Level**
    * Formal
    * Informal
7. **Narrative Perspective**
    * First Person
    * Second Person
    * Third Person
8. **Genre**
    * Science Fiction
    * Fantasy
    * Mystery
    * Romance
9. **Persona**
    * Historian
    * Scientist
    * Fiction Writer
    * Journalist
    * Educator
    * Critic
    * Advisor
    * Debater
10. **Language Preference**
    * English
    * Spanish
    * French
    * German
11. **Complexity Level**
    * Simple
    * Intermediate
    * Advanced
12. **Structure**
    * Linear
    * Non-linear
13. **Argument Stance**
    * Pro
    * Con
    * Balanced
14. **Setting**
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
15. **Document Format**
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
16. **Constraints**
    * Word Count Limit
    * Time Period
    * Specific Themes
    * Specific Characters
    * Specific Settings
    * Specific Genres
    * Language Restrictions
    * Content Restrictions
17. **Detail Level**
    * High
    * Medium
    * Low
18. **Factuality**
    * Factual
    * Fictional
19. **Output Length**
    * Short
    * Medium
    * Long

## Without Options or Formatting

1. Objective
    * Inform
    * Entertain
    * Persuade
    * Educate
2. Target Audience
    * General Public
    * Children
    * Adults
    * Subject Matter Experts
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

# Prompt Generators

## Create Prompt

Generate a prompt to [PURPOSE]. The prompt should be optimized for a natural language processing large language model in
a format that is similar to the example output.

You will select the control tokens and keywords that will be used to generate the prompt.

Here is a list of control tokens for you to choose from and sections. If there is a more effective one that you can
think of, use that instead for the control token section.

You can also add additional control tokens per section if you think they are necessary. Having multiple control tokens
per section is fine, but try to use only one or two per section.

Mandatory control tokens:

* Objective
    * Target Audience
    * Output Format
    * Emotional Tone
    * Formality Level
    * Language
    * Output Length
    * Persona
    * Writing Style

List of possible control tokens:

1. Objective
    * Inform
    * Entertain
    * Persuade
    * Educate

    2. Target Audience
        * General Public
        * Children
        * Adults
        * Subject Matter Experts
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

**System Message:** (Text)

**Instructions:** (Text)

**Control Tokens**

* **[Objective]** option
    * **[Target Audience]** option
    * **[Output Format]** option
    * **[Emotional Tone]** option
    * **[Formality Level]** option
    * **[Language]** option
    * **[Output Length]** option
    * **[Persona]** option
    * **[Writing Style]** option
    * **[Token]** Option
        * Add tokens from the list or your own knowledge as necessary.

**Keywords:** [Text]

**Example Output:**

~~~
(Text)
~~~

"""