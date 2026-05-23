# Everyday AI Skills

Practical AI skills you can reuse for real-world day-to-day work.

This repository contains portable, instruction-first skill packs that can be used in Claude, ChatGPT, Gemini, and other LLM tools. Each skill includes a `SKILL.md` core instruction file and optional reference files to improve output quality.

## Why this repo exists

Most prompt examples online are one-off snippets. This repo focuses on reusable skills that are:

- Domain-aware
- Structured and easy to run
- Safer against hallucinations
- Easy to plug into project-based AI workflows

## Repository structure

Each skill lives in its own folder:

```text
<skill-name>/
  SKILL.md
  references/
    *.md
  <optional packaged file>.skill
  README.md
```

- `SKILL.md`: Main behavior and workflow instructions for the AI model.
- `references/`: Supporting files used by the skill when needed.
- `.skill`: Optional packaged format for tools that support importing skill bundles directly.
- `README.md` inside each skill: Tool-specific setup instructions and examples.

## Available skills

### 1) resume-tailor
AI-powered resume tailoring engine that edits an existing resume to align with a specific job description while preserving truthfulness and formatting intent.

Path: `resume-tailor/`

## Quick start (any AI tool)

1. Open the skill folder you want to use.
2. Copy the full content of `SKILL.md`.
3. Paste it into your AI tool's system/project/custom instructions area.
4. Upload any files from `references/` (recommended).
5. Provide your task inputs in chat (for example: resume + job description).

For exact steps for the resume-tailor skill, see [resume-tailor README](./resume-tailor/README.md).

## How to use this repo

You can use this repository in two ways:

1. Use skills directly from files
- Best for manual setup in Claude/ChatGPT/Gemini.
- Copy `SKILL.md`, upload `references/`, and start chatting.

2. Use packaged `.skill` files
- Best for platforms/tools that support direct skill import.
- Import the `.skill` file if your tool supports it.

## Contributing

Contributions are welcome. To add a new skill:

1. Create a new folder with a clear skill name.
2. Add `SKILL.md` with role, scope, process, constraints, and output format.
3. Add a `references/` folder for optional support docs.
4. Add a skill-level `README.md` with setup instructions for common AI tools.
5. Open a pull request with a short description and example use case.

## License

Add your preferred license in a `LICENSE` file (for example, MIT) so others can confidently reuse this work.
