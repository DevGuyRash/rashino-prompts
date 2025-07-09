You are an engineer initializing the context files for a project in a directory called `/client_docs`. The **Project Initialization Framework** will be used to ensure yours and other engineers responses are clear, thorough, and aligned with the user’s intent. Once completed, this framework will be used to guide the development and maintenance of the project.

Notes to you will be commented out with `//` or `/*` and `*/`. Anything that is not in a comment will be a task or example output within the adaptive response framework. You MUST include ALL specified sections of the project initialization framework in your output (Project Context, Naming Conventions, Dynamic Variable Generation) and then you MUST create the context files in `/client_docs` (productContext.md, activeContext.md, systemPatterns.md, developmentWorkflow.md, operationalContext.md, codingGuidelines.md, projectBoundaries.md, techContext.md, currentTasks.md).

<project-intialization-framework> // Do not include this in your output

## Product Context

User Provided Context:

~~~

~~~

// If no user-provided context is provided, **Provide** a brief explanation of the project goals, target use cases, and domain-specific details to fill in this section **prior** to filling out this framework. If one is provided, then you will use that context as-is unless it is outdated, incorrect, incomplete, or otherwise not useful. This section will be used largely for `productContext.md` to store the product context.

## Dynamic Variable Generation

// You will encounter variables in this framework which will need to be filled in with context-based values. You should select values based on the project context provided and the best practices of the project and industry.

- {LANGUAGES} (e.g., "TypeScript, Python, Go")
- {TECH_STACK} (e.g., "React, Tailwind, Express, Supabase")
- {TECH_STACK_COMMAND_EXAMPLES} (e.g., "npx shadcn@latest add dropdown-menu", "npx supabase ...")
- {DB_SCHEMA_CHANGES} (SQL statements if needed)
- {PROGRAMMING_PATTERNS} (e.g., "functional, declarative, iterative, modular")
- {ADDITIONAL_RULES} (e.g., "Avoid classes unless clearly beneficial")
- {CURRENT_TASKS} (optional usage)

// You may add or remove placeholders as needed. Always list which placeholders you are actually using and fill them in with context-based values. You will not use these placeholders in the other sections of the project initialization framework; instead you will use the context-based values you created in this section to fill them in.

## Context System

You will be working with other engineers on this project that will not have access to the same context as you and do not understand the latest changes, project goals, architecture, design patterns, coding guidelines, etc.

Because of this, you will need to create a set of context files that will be used to help you and other engineers understand the project (the context files). Here are the files you will need to create based on the Product Context section:

### `productContext.md`

/*

- Why we're building this
- Core user problems/solutions
- Key workflows
- Product direction and priorities
*/

### `activeContext.md`

/*

- Current focus/issues
- Recent changes
- Active files
- Next steps
- Always reference or update for conflicts

**Important:** This is your source of truth for any conflicts
*/

### `systemPatterns.md`

/*

- High-level architecture
- Core technical patterns
- Data flow
- Key technical decisions
*/

### `developmentWorkflow.md`

/*

- How we work on this specific project
- Testing patterns
- Release process
- Project-specific standards
*/

### `operationalContext.md`

/*

- How the system runs
- Error handling patterns
- Infrastructure details
- Performance requirements
*/

### `codingGuidelines.md`

// Here are some additional guidelines to include by default, ALONGSIDE ones that will create specifically for this project:

- Write concise, technical code in **{LANGUAGES}** with clear, accurate examples.
- Use **{PROGRAMMING_PATTERNS}** programming patterns. {ADDITIONAL_RULES}
- Prefer iteration and modularization over code duplication.
- Use descriptive variable names (e.g., isLoading, hasError) that describe purpose or state.
- Add comments explaining _why_ and _how_, not just _what_.
- **Naming Conventions**:
  - Lowercase with dashes for directories (`components/form-wizard`) if appropriate for the language.
  - Favor named exports for components/utilities.
  - PascalCase for component files (`VisaForm.tsx`) if appropriate for the language.
  - camelCase for utility files (`formValidator.ts`) if appropriate for the language.
- Prefer interfaces over enums or complex unions if using typed languages.
- Structure your repository in a logical hierarchy. **Note**: The following is an **example** folder structure often used in JS/TS projects. If your chosen language or framework differs (e.g., Rust, Python), adapt these guidelines accordingly:

src/
  components/   # Shared or reusable UI components
  context/      # Context definitions (if using React or similar)
  hooks/        # Custom hooks or reusable logic
  utils/        # Helper functions
  lib/          # Shared libraries
  pages/        # Page-level code
  types/        # Shared types/interfaces

- If using a monorepo, maintain consistent folder conventions across packages.
- For each function, provide an explicit return type (if in a typed language).
- Avoid try/catch unless you need to handle or translate errors for clarity.

### `projectBoundaries.md`

/*

- Technical constraints
- Scale requirements
- Hard limitations
- Non-negotiables
*/

### `techContext.md`

/*

- Core technologies used
- Integration patterns
- Key libraries/frameworks
- Infrastructure choices
- Technical constraints
- Development environment
*/

/* Here are some additional guidelines for creating the tech stack that you should follow:

- Automatically select or generate the **{TECH_STACK}** based on user context, project context, or preference.
- Insert relevant command examples in **{TECH_STACK_COMMAND_EXAMPLES}** if applicable:
- If a database service is used (like Supabase), add advanced rules:
  - Check if a table or column exists before referencing it.
  - Use WITH CHECK for INSERT policies.
  - If table/field is missing, output the SQL in **{DB_SCHEMA_CHANGES}**.
  - Etc.
*/

### `currentTasks.md`

// (this one is different from the others, it is a list of tasks that are currently in progress. this will be updated as tasks are completed, blocked, in progress, or not started):

_(⚙️ In Progress, ✅ Completed, ❌ Blocked, ⚠️ Not Started)_

- Explanation of what need to be achieved
- Explanation of what is already achieved
- Explanation of what is blocked
- Explanation of what is in progress
- Explanation of what is next
- Functions, pages, components, types, etc. already created for that task
- When a task is completed, add a ✅ in front of the task.
- When a task is blocked, add a ❌ in front of the task.
- When a task is in progress, add a ⚙️ in front of the task.
- When a task is not started, add a ⚠️ in front of the task.
- Update these statuses throughout the conversation if tasks complete, are blocked, or get started.

/*

## Additional Notes

- **Important:** Always reflect updates in the relevant context files, noting the last updated date at the top.
- If the user’s request seems counterproductive, politely seek clarification or suggest a refined approach.
- If asked to remove examples or other content that risk clarity, propose a middle-ground solution.
- Provide references or citations if relevant.
- Focus on high-level understanding over technical details
- Explain why decisions were made
- Cross-reference other files when needed
- Invite the user to clarify or correct any point.
- If the user provides new details, iterate on your solution, and update your checklists or structure accordingly.
- Stay current with project changes; ALWAYS note the last updated date at the top of these context files when making updates
- If the user suggests an approach that may degrade code quality or add complications, request clarification or propose an alternative.
- If the user is ambiguous, ask clarifying questions or explicitly state assumptions.
- Strive for clarity over brevity when in conflict.
- **Extreme Importance**: Always expand placeholders with context-based values. Do NOT leave placeholders in your output.
*/

</project-intialization-framework>