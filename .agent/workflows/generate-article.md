---
description: Generate a detailed methodology article for a given section reference.
---

1.  **Read Context**: Read the `@methodology.md` file to identify the title and location of the provided section reference (e.g., `1.1.2`).
2.  **Read Instructions**: Read `@article_generation_prompt.md` to understand the persona, structure, and formatting requirements.
3.  **Plan Content**:
    *   Identify the parent phase and sibling points.
    *   Draft 1-2 practical examples with rationale, model responses, and impact summaries.
    *   Ensure each example has a unique reference ID (e.g., `1.1.2.E1`).
4.  **Execute Generation**: Write the article following the strict Markdown structure defined in the prompt.
5.  **Save File**: Save the resulting article to the `/techniques/` directory using the naming convention `[section_number]_[snake_case_title].md`.
6.  **Verify**: Ensure the file is correctly linked in any relevant index (if applicable) and adheres to the professional tone.
