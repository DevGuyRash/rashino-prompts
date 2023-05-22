[INSTRUCTIONS] = "Create specialized instructions with the purpose of $[DESIGN]. You will create the instructions by creating a JSON in the format of $[FORMAT], filling in relevant keywords, control tokens, sections, and other information."

[DESIGN] = "{PROMPT}"

[CONTROL_TOKEN_SECTIONS] = [
    "Objective",
    "Target Audience",
    "Output Format",
    "Writing Style",
    "Emotional Tone",
    "Formality Level",
    "Narrative Perspective",
    "Genre",
    "Persona",
    "Language Preference",
    "Complexity Level",
    "Structure",
    "Argument Stance",
    "Setting",
    "Document Format",
    "Constraints",
    "Detail Level",
    "Factuality",
    "Output Length"
]

[REQUIRED_CONTROL_TOKEN_SECTIONS] = [
    "Persona",
    "Objective",
    "Target Audience",
    "Output Format",
    "Output Length",
    "Emotional Tone",
    "Formality Level",
    "Writing Style",
    "Constraints"
]

[CONSTRAINTS] = [
    "Choose the appropriate values for each field in the json",
    "Include relevant control tokens per section and keywords to guide the output",
    "Expand upon sections and control tokens as necessary to enhance the prompt",
    "Limit 1-2 control tokens per section, unless required",
    "Control token values should only have the name, no formatting",
    "Provide context, constraints, persona, and background information to the large language model in the "System Message" section, directed at the language model",
    "Instruct the large language model inside the "User Instructions" section with specific and detailed instructions on what to do, how to do it (by making use of the control tokens and information), and what to focus on (the keywords)",
    "Only produce the desired output and nothing else, unless user input is required",
    "Format=$[FORMAT]",
]

[FORMAT] = 
{
    "System Message": "{System Message}",
    "User Instructions": "{Instructions to the LLM}",
    "Current Subject": "{SUBJECT}",  // Leave this as is
    "Control Tokens": {
        "Persona": "{CONTROL TOKEN}",
        "Objective": "{CONTROL TOKEN}",
        "Target Audience": "{CONTROL TOKEN}",
        "Output Format": "{CONTROL TOKEN}",
        "Output Length": "{CONTROL TOKEN}",
        "Emotional Tone": "{CONTROL TOKEN}",
        "Formality Level": "{CONTROL TOKEN}",
        "Writing Style": "{CONTROL TOKEN}",
        "Constraints": {
            "Token Name": "{CONTROL TOKEN}",
            "Token Name": "{CONTROL TOKEN}"
            // Continue adding relevant constraints
        }
        // Continue adding relevant control token sections and control tokens for those sections
    },
    "Keywords": [
    "keyword",
    "keyword",
    "keyword"
    // Continue adding relevant keywords
    ],
    "Example Output": "{Example output that utilizes the control tokens and keywords to produce a structured, high-quality, relevant output}"
}

Instructions($[CONSTRAINTS], $[CONTROL_TOKEN_SECTIONS], $[REQUIRED_CONTROL_TOKEN_SECTIONS])