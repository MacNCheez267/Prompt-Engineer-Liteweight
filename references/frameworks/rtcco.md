# RTCCO framework

## Components

- **Role:** The perspective or expertise the assistant should use, if a role would improve the result.
- **Task:** The action the assistant should perform.
- **Context:** Background, source material, or situation relevant to the task.
- **Constraints:** Boundaries and requirements, including what to include or avoid.
- **Output:** The requested deliverable and its format.

## When to use

Use RTCCO as the general-purpose default for prompts with several requirements, meaningful background, constraints, or a deliverable that needs definition. It helps expose gaps without requiring every section to be filled.

## How to adapt

Use only components that clarify the user's request. Do not invent a role, context, constraint, or output format. Keep unsupported or nonessential fields optional; ask about a missing field only when it materially affects the result. Combine or omit headings when they would create repetition.

## Reusable template

> **Role:** [Perspective or expertise, if useful]
>
> **Task:** [What to do]
>
> **Context:** [Relevant background or source material]
>
> **Constraints:** [Requirements and boundaries]
>
> **Output:** [Deliverable and format]
