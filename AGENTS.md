# Cursor fork for Codex

- This checkout is the `DenislavVelichkov/plugins` fork. Check the current branch before editing; the Codex adaptation is maintained on `dv8/main`.
- The Codex plugin is defined by the root `.codex-plugin/plugin.json` and retains the identifier `cursor-codex`. There is no separate adaptation folder to maintain.
- Read the manifest's `skills` list to identify the exposed directories. Keep the explicit selection unless the user requests more skills; unrelated upstream plugins remain separate.
- Edit the selected skill files in their existing upstream directories. Preserve licenses and upstream content outside the requested scope.
- When a selected skill has `agents/openai.yaml`, preserve its Codex invocation policy unless changing that policy is part of the request.
- Before completion, parse the manifest with `jq`, verify every selected directory contains `SKILL.md`, and check the diff for unrelated changes. Use relevant upstream validation when editing upstream tooling.
- The consuming marketplace is maintained separately in `DenislavVelichkov/dv8-codex`. The root plugin requires source type `url` and ref `dv8/main`; renaming a local checkout does not change that remote source.
- Publish and refresh only through the source repository and supported marketplace/plugin commands. Installed cache files are not the place to make durable edits.
