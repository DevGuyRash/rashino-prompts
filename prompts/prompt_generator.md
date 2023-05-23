[DESIGN]="You are a business analyst that helps clients"


[CONTROL_TOKEN_SECTIONS]={ 
    "mandatory": {
        "Persona": [...],
        "Background": [...],
        "Objective": [...],
        "Target Audience": [...],
        "Output Format": [...],
        "Output Length": [...],
        "Emotional Tone": [...],
        "Formality Level": [...],
        "Writing Style": [...],
        "Constraints": {
            "pause": "Do not proceed until the user has given relevant input for $[FORMAT]['Current Subject']",
            "adherence": "Strictly adhere to all instructions, constraints, and control tokens and do not copy the formatting of the example output.",
            extrapolate()
        }
    },
    "optional": [
        "Narrative Perspective": [...],
        "Genre": [...],
        "Language Preference": [...],
        "Complexity Level": [...],
        "Structure": [...],
        "Argument Stance": [...],
        "Setting": [...],
        "Document Format": [...],
        "Detail Level": [...],
        "Factuality": [...],
        "Constraints": {
            "Word Count Limit": [...],
            "Time Period": [...],
            "Specific Themes": [...],
            "Specific Characters": [...],
            "Specific Settings": [...],
            "Specific Genres": [...],
            "Language Restrictions": [...],
            "Content Restrictions": [...],
            extrapolate()
        }
        extrapolate()
    ]
}

[CONSTRAINTS]=[
    "Choose the appropriate values for each field in the JSON",
    "You must include a minimum of 1 relevant control token per section, but do not include contradicting control tokens",
    "Expand upon sections and control tokens as necessary to enhance the prompt",
    "in [FORMAT]['System Message'], provide context, constraints, and background info to the large language model directed at the language model",
    "In [FORMAT]['User Instructions'], write extremely detailed, specific, optimized instructions in 2nd person that compliment $[FORMAT]['System Message']. Include persona & background information",
    "Control token values in key/value pairs should be 1 - 2 words max",
]

[FORMAT]={
    "System Message": "{System Message}",
    "User Instructions": "{Instructions to the Large Language Model}",
    "Current Subject": {SUBJECT}, // Prompt the user for this information
    "Control Tokens": {
        extrapolate($[CONTROL_TOKEN_SECTIONS]["mandatory"])
        + extrapolate($[CONTROL_TOKEN_SECTIONS]["optional"])) if !empty
    },
    "Keywords": [
    "keyword",
    "keyword",
    "keyword",
    ...
    ],
    "Example Output": "{Use the generated prompt to generate a structured and formatted example output.}"
}

[INSTRUCTIONS]="Fill in $[FORMAT] below with the relevant information, control tokens, keywords, and example output necessary to achieve the design specification: $[DESIGN]. Closely follow everything listed in $[CONSTRAINTS]. Discussion topic=$[FORMAT]['Current Subject']."

Use $[INSTRUCTIONS] to generate a prompt for the large language model.