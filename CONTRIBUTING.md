# Contributing

Thanks for your interest! This is a curated collection, so contributions are held to a quality bar.

## Adding a workflow

1. **Sanitize it first** — remove all credentials, `pinData`, `instanceId`, webhook UUIDs, and any personal data. See [SECURITY.md](SECURITY.md) for the full standard.
2. **Name it clearly** — `kebab-case-describing-the-outcome.json`, placed in the matching `workflows/<category>/` folder.
3. **Test it imports** — it must load into a current `n8nio/n8n` instance without error.
4. **Run validation locally**:
   ```bash
   python3 scripts/validate.py
   ```
5. Open a pull request. CI will re-validate and run a secret scan.

## What gets accepted

- Production-quality workflows with a clear real-world outcome
- Current node types and AI models (no deprecated `function`/`itemLists` nodes, no `gpt-3.5`)
- At least a trigger and one meaningful action

## What doesn't

- Anything containing secrets (auto-rejected by CI)
- Trivial 2–3 node stubs or auto-generated placeholder names
- Workflows on dead/removed APIs
