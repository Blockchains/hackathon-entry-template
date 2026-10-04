# AGENTS.md: hackathon-entry-template

Instructions for AI coding agents (Grok, Cursor, Claude Code, Codex, Copilot and others) working **in** this repo or **using it as a building block**. Humans: see [README.md](README.md).

## What this is

Generic hackathon entry template: README skeleton (problem, solution, architecture, what was built), docs/SUBMISSION.md checklist, .env.example, and CI that scans for secrets and auto-detects Node, Python or Foundry to build and test.

- Kind: template · stability: `stable` · licence: MIT
- Machine-readable manifest: [`blocks.json`](blocks.json) (schema: [BLOCKS-SCHEMA](https://github.com/Blockchains/.github/blob/main/docs/BLOCKS-SCHEMA.md))
- How it fits with the other Blockchains repos: [Build with Blocks](https://github.com/Blockchains/.github/blob/main/docs/BUILD-WITH-BLOCKS.md)

## Setup

```bash
cp .env.example .env
```

## Build and test

```bash
# CI auto-detects: npm test / pytest / forge build && forge test
```

## Structure

| Path | What |
|---|---|
| `README.md` | write-up skeleton with <placeholders> |
| `docs/SUBMISSION.md` | submission checklist |
| `src/` | your code |
| `.github/workflows/ci.yml` | secret scan + auto build/test |

## Conventions

- Replace every `<placeholder>`; CI warns if `<Project name>` remains.

## Extension points

- Add your stack's manifest at the repo root so CI picks it up.

## Do

- List what was built during the hackathon vs pre-existing.

## Don't

- Invent data, mock network responses in shipped code, or hard-code values that should come from the live source; every repo here is 'no mocks, real data'.
- Commit secrets, keys or `.env` files. Run `gitleaks` before pushing; CI and the org policy reject leaks.

## Using it from another project

- **Use this template** (git): `GitHub template`
- **.github/workflows/ci.yml** (file): `gitleaks + auto-detected build/test (package.json, requirements.txt/pyproject.toml, foundry.toml)`

See the README section [Use as a building block](README.md#use-as-a-building-block) for a copy-paste example.

## Related blocks

- [Blockchains/hackathons](https://github.com/Blockchains/hackathons): link the tracker issue in the README header
- [Blockchains/blockchainlab-starters](https://github.com/Blockchains/blockchainlab-starters): start the code from a starter
- [Blockchains/grokhack-submissions](https://github.com/Blockchains/grokhack-submissions): Grok Hack specific template
