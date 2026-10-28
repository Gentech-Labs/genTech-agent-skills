# GenTech Agent Skills

**176 skills for Hermes Agent** — 59 categories, one folder per skill. Each skill is a `SKILL.md` with
YAML frontmatter stating *when* it fires, plus its own `references/` and `scripts/` where the procedure
needs them.

This is the public mirror of the skill shelf our own agent fleet runs on. It is a working set, not a
catalogue: every skill here exists because a task failed once and the lesson had to survive the session.

---

## What's in here

| Category | Skills | What it covers |
|---|---:|---|
| `gentech-ops` | 44 | build queue, handoff mesh, cron routing, gateway recovery, deployments, session hygiene |
| `devops` | 17 | containers, destructive-write guards, safe restarts, health monitoring, git conflicts |
| `agent-kit` | 14 | audits, cron health standards, falsifiable tests, preflight, self-evolution |
| `gentech` | 10 | voice lane, daily sync, wallet and credential handling, family hubs, portfolio deploys |
| `research` | 8 | arXiv, direct model calls, domain recon, scraping, freelance marketplaces |
| `defi` | 6 | LP venue mechanics, pool analytics, on-chain readers, arbitrage |
| `creative` | 6 | brand assets, diagrams, video frames, image and meme generation |
| `security` | 4 | code and privacy audits, secret handling in chat, OSINT |
| `finance` | 4 | three-statement models, DCF, price feeds, x402 payments |
| `agent-economy` | 3 | marketplace integration, listings, on-chain agent execution |
| `agent-coordination` | 3 | agent messaging, handoff mesh, per-group workers |

…and 48 more categories carrying 1–2 skills each — memory, media, career, travel, gaming, MCP, git,
blockchain, Telegram publishing, identity.

**Counts measured from this repository on 2026-10-28: 176 `SKILL.md` across 59 categories.** If a
number here drifts, the tree is the truth — the README is a summary, not an index.

---

## Install

**Whole shelf** into a Hermes profile:

```bash
git clone https://github.com/Gentech-Labs/genTech-agent-skills.git
cp -r genTech-agent-skills/skills/* ~/.hermes/profiles/<profile>/skills/
```

**One skill**, if you only want the lesson you came for:

```bash
cp -r genTech-agent-skills/skills/gentech-ops/build-queue \
      ~/.hermes/profiles/<profile>/skills/gentech-ops/
```

Skills are read at **load time**, so a copied skill takes effect on the next session — no restart, no
service reload.

---

## What a skill looks like

`skills/gentech-ops/build-queue/SKILL.md` opens like this — real frontmatter, not an illustration:

```yaml
---
name: build-queue
description: "V4 autonomous build queue — agent works Easy→Hard, saves brain notes at stopping
  points, auto-switches tasks."
tags: [build, automation, pipeline, queue, agent-kit, autonomous, v4]
trigger: "When the user says 'start build list', 'run the queue', wants autonomous task
  processing, or the V4 Build Queue Tick cron fires (every 30m)."
version: 4.0.0
author: Gentech Labs
---
```

`trigger` is the field that matters. A skill without one is documentation; a skill with one is a
procedure the agent reaches for on its own.

---

## Layout

```
skills/<category>/<skill-name>/SKILL.md     the procedure
                             references/    deeper notes, loaded on demand
                             scripts/       runnable checks and helpers
skills/README.md                            how the shelf is laid out and synced
docs/                                       field notes: gateway troubleshooting, memory rules
cron/  erc-8004/  examples/  vault-structure/   supporting material
```

---

## How these get written

- **From a measured failure, not a docs page.** Most skills open with the incident that produced them —
  the date, the command that lied, the number that was wrong.
- **A check that cannot go red is a bug.** Two skills exist only to make a guard provable:
  `falsifiable-tests` and `guard-verification`.
- **Portable paths.** Skills reference `${VAULT_DIR}` rather than an absolute path, so the same folder
  works on a laptop and a VPS. `skills/README.md` documents the one trap: the variable has to be
  defined on the seat, or every command expands to nothing and fails silently.

---

Built by [GenTech Labs](https://github.com/Gentech-Labs) · agent infrastructure that holds up under money
