---
description: Generate a detailed sub-article for a specific example within an article.
---

1.  **Identify Example**: Receive the example reference ID (e.g., `1.1.2.E1`).
2.  **Read Context**: 
    *   Find the main article file in the `/techniques/` directory that contains this example (e.g., `1.1.2_establishing_rules_of_engagement.md`).
    *   Identify the base model or scenario context from the main article to ensure consistency.
3.  **Read Instructions**: Read `@example_explanation_prompt.md` to understand the specific requirements for detailed example breakdowns.
4.  **Execute Generation**: Write the detailed sub-article explaining the technical nuances, variant prompts, and deep-dive mitigation strategies for this specific example.
5.  **Save File**: Save the sub-article to the `/techniques/examples/` directory using the naming convention `[example_id].md`.
6.  **Verify**: Ensure the sub-article links back to the main article and uses the correct authoritative tone.
