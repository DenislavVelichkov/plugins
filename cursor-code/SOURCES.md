# Codex skill sources

The Codex adaptations live in `cursor-code/` on the `dv8/main` branch of this fork. They were copied from `DenislavVelichkov/dv8-codex` without changing the skill files or licenses.

These two skills were originally imported from https://github.com/DenislavVelichkov/plugins at commit `60c641e4fad674784b30abcf9f8915dea39df38d`.

- `thermo-nuclear-code-quality-review`: `cursor-team-kit/skills/thermo-nuclear-code-quality-review/SKILL.md`. MIT, copyright 2026 Cursor.
- `unslop`: `pstack/skills/unslop/SKILL.md`. MIT, copyright 2026 Lauren Tan. The newer locally supplied update's upstream revision has not been established; the commit above records the original import.

Codex invocation policy is defined in each skill's `agents/openai.yaml`. Code quality review requires explicit invocation. Unslop allows implicit invocation.

Each skill directory contains its upstream license. No other skills or agents from the fork are bundled. These are real files; updating the upstream skills does not automatically update these adaptations.
