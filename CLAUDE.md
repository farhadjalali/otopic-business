# Otopic — Business Knowledge Base

This is a **standalone repository**. It lives beside the `otopic/` source tree on disk, but it is **fully separate from the code**: it has (or will have) its own git history and remote.

**Hard boundary: business vs. technical.**
- This repo holds **everything non-code** about Otopic: strategy, market, pricing, product thinking, and decisions.
- It is **not** the place for code, build config, infra, or implementation detail. Those live in the `otopic/` repo (`web/`, `api/`, `ios/`, `database/`, etc.) and are governed by their own `CLAUDE.md`.
- Do not pull technical context from `otopic/` into business docs, and do not let business strategy leak into code. Keep them apart on purpose.

## What this is

A markdown + YAML knowledge base built around one loop:

**capture fast → review → promote to the right home.**

```
 idea  ──►  inbox/  ──►  (weekly review)  ──►  strategy / product / market / pricing / decisions
```

See [README.md](./README.md) for the full loop and the folder-by-folder source-of-truth table.

## Where things live

| Folder | Holds | Source of truth for |
| --- | --- | --- |
| `inbox/` | Raw, unsorted capture | nothing — staging area |
| `strategy/` | Vision, positioning, customers, model, GTM, risks, governance, Sapilon synergy | what we're building and why |
| `product/` | Value prop, use-cases, personas, idea drafts | what the product is |
| `market/` | Competitor deep-dives, the matrix, observations | the landscape |
| `pricing/` | Current model, assumptions, experiments | how we charge |
| `decisions/` | Lightweight decision log (dated, numbered) | why we chose X |
| `research/` | Raw notes, links, founder questions | reference |
| `templates/` | Reusable doc skeletons | reuse |
| `archive/` | Superseded / rejected, kept for history | history |

## Conventions

- **Markdown for prose, YAML for data.** Anything rendered as a table or list elsewhere (competitor matrix, pricing assumptions) is YAML so there's one structured source.
- **`_TEMPLATE.md`** in a folder is a copy-me starter — never edit it as content; copy it.
- **Dates in filenames** for time-stamped things (`inbox/`, `decisions/`, `archive/` snapshots): `YYYY-MM-DD-slug`.
- **One thing per file.** If a file grows a second topic, split it.
- `decisions/` entries are **numbered and dated** (`NNNN-slug.md`) — append, don't rewrite history.

## Working in this repo

- When asked to capture an idea, default to a new file in `inbox/` — don't agonize over taxonomy.
- When promoting from `inbox/`, move the note into the right folder above and delete/archive the inbox copy so the inbox stays empty = reviewed.
- Prefer editing the existing source-of-truth file over creating a parallel one; check the table above first.
- Keep prose tight and decision-oriented; this is a founder's working KB, not marketing fluff.
