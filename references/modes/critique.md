# Critique mode

Identify the most consequential weaknesses in the prompt, such as unclear goals, missing material context, conflicting constraints, unspecified output, or unnecessary structure. Tie each observation to the text and explain its likely effect briefly. Do not over-critique harmless omissions. Offer a concise clarifying question when an ambiguity materially affects the result. Include a revised prompt only if the user asks for one or if a faithful revision would be useful; label it separately and do not silently resolve material ambiguity.

## Example

**Before**

> Make a plan for the project.

**Critique**

- **The deliverable is underspecified:** “plan” could mean a schedule, task list, or strategy, so responses may vary substantially.
- **Key context is missing:** the project and its goal are not identified.

**Question**

> What project is the plan for, and what kind of plan do you need?

A revision should wait for the answer because the missing information changes the task.
