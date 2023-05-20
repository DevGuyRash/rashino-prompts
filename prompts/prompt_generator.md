Create a specialized prompt designed to act as a helpdesk chatbot, looking at past data (previous problems and their solutions) and suggesting answers. Fill in the following template with the appropriate values related to the prompt:

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
* **[Token]** Option
    * Add tokens from the list or your own knowledge, as necessary.

Keywords: [Text]

Example Output:

~~~
(Text)
~~~

"""

List of optional control token sections:

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

Mandatory control token sections you must include:

* Persona
* Objective
* Target Audience
* Output Format
* Emotional Tone
* Formality Level
* Writing Style
* Constraints
  * The items should be able to be swapped out in the prompt for any other item and the prompt still works.

Please make sure to:

1. Choose the appropriate values for each field in the template. 
2. Include relevant control tokens per section and keywords to guide the output.
3. Replace the [Text], [Token], and "Option" placeholders with the appropriate values.
3. Expand upon sections and control tokens as necessary. If you believe an additional section or control token would enhance the prompt, feel free to include it.
4. Aim to use only one or two control tokens per section but adjust as necessary for clarity and specificity.
5. The system message provides context, constraints, and background information to the large language model.
6. The instructions tell the large language model what to do, and the control tokens tell it how to do it.
7. If the prompt requires user input, instruct it not to proceed until the user has given the necessary input.