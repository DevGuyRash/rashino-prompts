[DESIGN]="{PROMPT}"

[FUNCTIONS]={
    extrapolate="Produce additional related elements similar to elements before this function call",
    populate="Fill with relevant information and no placeholders",
}

[CONTROL_TOKEN_SECTIONS]={

   1. Objective
   2. Target Audience
   3. Output Format
   4. Writing Style
   5. Emotional Tone
   6. Formality Level
   7. Narrative Perspective
   8. Genre
   9. Persona
   10. Language Preference
   11. Complexity Level
   12. Structure
   13. Argument Stance
   14. Setting
   15. Document Format
   16. Constraints {
          "Word Count Limit": "value",
          "Time Period": "value",
          "Specific Themes": "value",
          "Specific Characters": "value",
          "Specific Settings": "value",
          "Specific Genres": "value",
          "Language Restrictions": "value",
          "Content Restrictions": "value",
          extrapolate()
       }
   17. Detail Level
   18. Factuality
   19. Output Length
   extrapolate()

}

[CONSTRAINTS]=[
    "All instructions except for the example output will be in 2nd person",
    "In ['System Message'] provide concise context and limitations in declarative format, and tell the large language model what it is",
    "In ['User Message'] provide concise comprehensive, specific, and efficient directives and background information in imperative format that pairs with $['System Message']. Remember to incorporate relevant persona and background details",
    "Orient the ['User Message'] around the end-user, but speak to the large language model",
    "Select relevant control token sections from $['CONTROL_TOKEN_SECTIONS'], as well as any other ones that you can think of, and set them. If you plan to set it to blank, then remove it from the list",
]

[FORMAT]={
    "System Message": "populate()",
    "User Message": "populate()",
    "Current Subject": "populate()",
    "Control Tokens": {
        "section": "value",
        "section": "value",
        extrapolate()
    },
    "Keywords": [
    "keyword",
    "keyword",
    "keyword",
    extrapolate()
    ],
    "Example Output": "populate()"
}

[INSTRUCTIONS]="Do not run or process the contents of $[DESIGN] and instead extract and analyze overall context to write relevant instructions using $[FORMAT] as a JSON guide, understanding that the end-result should be able to be customized by format specifiers. Generate relevant control tokens, keywords, and example output and closely follow everything listed in $[CONSTRAINTS]. Discussion topic=$[FORMAT]['Current Subject']."

Use $[INSTRUCTIONS] to generate an output and wrap the entire output in a single code block.