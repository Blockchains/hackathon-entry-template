# <Project name>

> One-sentence pitch: what it does and for whom.

**Hackathon:** <name + link> · **Track(s):** <tracks / sponsor bounties> · **Team:** <names / handles>
**Demo video:** <link (2–5 min)> · **Live demo:** <link> · **Tracker issue:** <Blockchains/hackathons#N>

## Problem
What hurts today, for whom, and why existing options fall short.

## Solution
What we built. Screenshot or diagram in `docs/`.

## How it works
- Architecture: frontend / backend / contracts / agents
- Chains & contracts: network, addresses, verified source links
- Sponsor tech used (and exactly where in the code)

## What was built during the hackathon
List what is new vs. pre-existing (many hackathons require this).

## Run it locally
```bash
git clone <repo>
cd <repo>
# install + run steps
```
Copy `.env.example` to `.env` and fill in values — **never commit `.env` or keys**.

## Challenges & what's next
<!-- blocks:start -->
## Use as a building block

> **For AI agents and builders:** read [`AGENTS.md`](AGENTS.md) (setup, commands, structure, rules), [`llms.txt`](llms.txt) (doc map) and the machine-readable [`blocks.json`](blocks.json) ([schema](https://github.com/Blockchains/.github/blob/main/docs/BLOCKS-SCHEMA.md)). How all Blockchains blocks fit together: **[Build with Blocks](https://github.com/Blockchains/.github/blob/main/docs/BUILD-WITH-BLOCKS.md)** · org catalogue: [https://blockchains.github.io/blocks.json](https://blockchains.github.io/blocks.json).

**What it exports**

| Export | Type | Install / access |
|---|---|---|
| `Use this template` | git | `GitHub template` |
| `.github/workflows/ci.yml` | file | `gitleaks + auto-detected build/test (package.json, requirements.txt/pyproject.toml, foundry.toml)` |

**Minimal example**

```bash
gh repo create my-entry --template Blockchains/hackathon-entry-template --public --clone
cd my-entry && cp .env.example .env   # never commit .env
```

**Inputs → outputs**

- In: `your code` (src/)
- Out: `entry repo with CI` (repo)

**Composes with**

- [Blockchains/hackathons](https://github.com/Blockchains/hackathons): link the tracker issue in the README header
- [Blockchains/blockchainlab-starters](https://github.com/Blockchains/blockchainlab-starters): start the code from a starter
- [Blockchains/grokhack-submissions](https://github.com/Blockchains/grokhack-submissions): Grok Hack specific template

**Versioning & stability:** `stable`. Template; changes affect new entries only.
<!-- blocks:end -->

## License
MIT — see [LICENSE](LICENSE).

---
<sub>Created from [Blockchains/hackathon-entry-template](https://github.com/Blockchains/hackathon-entry-template). Submission checklist: [docs/SUBMISSION.md](docs/SUBMISSION.md).</sub>
