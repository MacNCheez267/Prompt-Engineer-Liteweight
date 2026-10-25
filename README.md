# Prompt Engineer Liteweight Skill

Compact guide for assessing and revising prompt text while preserving the user’s intent. Includes clear boundaries, distinct 5 revision modes, and 3 practical framework guidance. Well suited for everyday prompt editing.

## How to Use

Provide the prompt and a revision mode: Polish, Refine, Shorten, Restructure, or Critique.

Modes may be combined. If none is specified, the skill defaults to Refine. It recommends a framework only when one would improve clarity.

## Workflow

1. Identify the user's request.

2. Assess the initial prompt using five dimensions: clarity, specificity, context, completeness, and structure.

3. Ask one concise question if a material ambiguity prevents a faithful revision; otherwise, proceed with a labeled assumption or leave the detail open.

4. Recommend a suitable framework, or none.

5. Revision of the prompt.

6. Check that the result preserves the user’s intent and requirements without adding unsupported details.

7. Present the revised prompt. Assessment score and change summary are separate.

```mermaid
graph TD;
    Identify-->Assess;
    Assess-->Question;
    Assess-->Recommend;
    Question-->Recommend;
    Recommend-->Revision;
    Revision-->Check;
    Check-->Output;
```

## Modes

| Mode | Example |
|------|---------|
| **Polish** | Correct grammar, spelling, and punctuation; address awkward wording with minimal changes. |
| **Refine** | Improve clarity and effectiveness while preserving intent. |
| **Shorten** | Remove redundancy while keeping essential requirements and constraints. |
| **Restructure** | Reorganize for readability without changing requirements. |
| **Critique** | Identify the main weaknesses. Include a revised prompt only when requested or when a faithful revision would materially help. |

## Frameworks

| Framework | Example |
|-----------|---------|
| **RTCCO** | General-purpose choice when the prompt has several requirements or needs explicit background, boundaries, and a defined deliverable. |
| **CO-STAR** | Suits writing, teaching, and communication when audience, style, or tone materially shape the result. Keep style and audience optional unless supplied; ask if missing details are consequential. |
| **RTF** | Suits simple, focused prompts where role, task, and format suffice. |

## Release Date
> October 24, 2026

## License
> [MIT License](LICENSE).

## Compatible Agents
> [OpenAI; (Codex | ChatGPT)](https://openai.com)
