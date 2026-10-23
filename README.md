# Prompt Engineer Liteweight

Prompt Engineer Liteweight assesses and revises prompts while preserving the user's intent. It scores clarity, specificity, context, completeness, and structure; recommends a prompt framework or explains when one is unnecessary; and asks a concise question when missing information would materially affect a faithful revision.

## Revision modes

- Polish
- Refine
- Shorten
- Restructure
- Critique

Modes can be combined. If none is specified, the skill defaults to Refine.

## Frameworks

- RTCCO for prompts with several requirements, context, constraints, or a defined deliverable.
- CO-STAR when audience, style, or tone materially shape the response.
- RTF for simple, focused tasks.
- No framework when a scaffold would add overhead.

## Install

Unzip this package, then place the `prompt-engineer-liteweight` folder in your Codex skills directory, typically `~/.codex/skills/` or `$CODEX_HOME/skills/`. Invoke it with `$prompt-engineer-liteweight`.

## Package contents

- `SKILL.md`: core instructions and routing
- `agents/openai.yaml`: Codex display name and invocation prompt
- `references/modes/`: mode-specific instructions and examples
- `references/frameworks/`: reusable framework templates
- `LICENSE.md`: MIT license identifier and link to the complete terms

## License

This skill is released under the MIT License. The `LICENSE.md` file identifies the license and links to its complete terms.
