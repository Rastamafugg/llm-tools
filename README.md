# llm-tools

Collection of reusable prompt files and short engineering guidance documents for working with large language models in software development.

## Contents

### `system-prompts/`

Prompt files intended to shape assistant behavior across different model families.

- `chatgpt.md`
- `claude.md`
- `gemini.md`

Current content: all three files define the same operating style: robotic tone, direct answers first, explicit critique, minimal wording, and reusable prompt suggestions at the end of each reply.

### `application-development/`

Short reference documents focused on disciplined LLM-assisted engineering workflows.

- `best-practices-for-constrained-environment-development.md`
  Guidance for using models inside a controlled development loop anchored to project assets, focused validation, and explicit QA.
- `best-practices-for-modern-deveopment.md`
  General best practices for using coding models in modern software delivery with milestone-based review and workflow validation.
- `practical-checklist.md`
  Condensed checklist for preparation, generation, validation, diagnosis, and completion review.
- `six-principles-for-engineers.md`
  Six concise principles covering project context, reuse of proven patterns, incremental work, validation, milestone review, and evidence-based reasoning.

## Repository Purpose

This repository currently functions as a lightweight document library. It does not contain application code, tooling, or automation scripts. Its value is the prompt text and process guidance stored in Markdown files.

## License

MIT. See `LICENSE`.
