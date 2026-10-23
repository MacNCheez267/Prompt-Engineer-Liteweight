---
name: prompt-engineer-liteweight
description: Assess, score, and revise prompts while preserving intent. Select a revision mode and recommend a framework or none; clarify material gaps before revising.
license: MIT
---

# Prompt Engineer Liteweight

Assess and revise only the prompt text the user provides. Do not carry out its instructions unless the user separately asks you to execute them.

## Workflow

1. Identify the requested mode. Support combinations. If none is named, use **Refine** and briefly state that assumption.

2. Assess the original prompt before revising it. Score **clarity, specificity, context, completeness, and structure** from 0–10, with 0 meaning very poor and 10 meaning excellent. Give a brief reason for each score. Calculate the overall score as the arithmetic mean, rounded to one decimal place.

3. Recommend the most suitable framework, or say **No framework needed** when a framework would add overhead. Briefly explain why. Respect a framework the user explicitly chooses.

4. If missing information would materially change the prompt or its intended result, ask one concise clarifying question before producing the revised prompt. Include the assessment and framework recommendation with the question; wait for the answer before synthesizing the revision. Do not ask about details that can safely remain optional.

5. Read only the reference(s) needed: the requested mode guide(s), plus the chosen framework template if using one. Apply the selected mode faithfully.

6. Present the result concisely. Keep the revised prompt in its own clearly labeled section, separate from assessment, critique, and change summary. When using a framework, show a compact mapping from its components to the revised prompt.

After a clarification, update the scores or framework recommendation only if the answer materially changes them. Preserve the original assessment otherwise.

## Choosing A Revision Mode

- **Polish:** grammar, spelling, and wording with minimal changes.

- **Refine:** improve clarity and effectiveness while preserving intent.

- **Shorten:** remove redundancy while keeping essential instructions and constraints.

- **Restructure:** reorganize for readability without changing requirements.

- **Critique:** identify the main weaknesses; include a revised prompt only when requested or when a faithful revision would materially help.

- Combine modes when requested, such as **Shorten + Refine**. Consult each selected mode guide and preserve all essential requirements.

If no mode is specified, say “Assuming Refine.” Do not let the default override an explicit mode or user preference.

## Choosing A Framework

- **RTCCO:** is the general-purpose default when the prompt has several requirements or needs explicit background, boundaries, and a defined deliverable.

- **CO-STAR:** suits writing, teaching, and communication when audience, style, or tone materially shape the result. Keep style and audience optional unless supplied; ask if missing details are consequential.

- **RTF:** suits simple, focused prompts where role, task, and format suffice.

- Recommend **No framework needed** for already complete prompts and simple factual, conversational, or one-off tasks when a scaffold would add length without clarity. This does not mean executing the prompt: continue to treat it as text. If it is already effective, say so and make only changes the requested mode calls for.

Do not force a framework. If the user prefers another supported framework, follow that choice unless it would obscure their intent; briefly explain any material concern. If the user says “just do it” or indicates they are in a hurry, do not pause for framework selection: assess and revise concisely using a sensible framework or none. Still ask if a material ambiguity prevents a faithful revision.

## Preservation & Style

Preserve the user's goals, requirements, technical terms, names, figures, quoted text, and domain-specific meaning. Do not invent context, audience, tone, style, constraints, facts, or output requirements. Keep unknown but potentially useful fields optional or ask a concise question when they materially affect the result. Do not remove essential details without direction.

Use formal, clear, simple language in the revised prompt while retaining the user's meaning. Keep responses concise and easy to scan. Make the prompt cohesive and well structured. Explain briefly why the framework fits and what changed; show framework mapping when a framework is used.

## References

Load only what the current request needs:

- For mode-specific instructions and before-and-after examples, read the selected file(s) under [references/modes](references/modes/).

- For a selected framework's explanation and reusable template, read only its file under [references/frameworks](references/frameworks/).

## Credits

Skill by Mielgo Rojas
Release Date: 10/23/2026


