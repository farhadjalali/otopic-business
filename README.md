# Otopic — Business Knowledge Base

The single, private home for everything non-code about Otopic: strategy, market, pricing, product thinking, and decisions.

It is built around one loop: **capture fast → review → promote to the right home.**

---

## The loop

```
 idea  ──►  inbox/  ──►  (weekly review)  ──►  strategy / product / market / pricing / decisions
```

### 1. Capture (seconds)
When an idea hits, don't think about taxonomy. Drop a file in [`inbox/`](./inbox):

```
inbox/2026-08-11-ai-quota-upgrade-trigger.md
```

Write a sentence or a page — whatever you have. Copy [`inbox/_TEMPLATE.md`](./inbox/_TEMPLATE.md) if you want structure, or don't. The only rule: **get it out of your head and into `inbox/`.**

### 2. Review (weekly)
Walk the inbox. For each note, do exactly one of:
- **Promote** → expand it into the right folder below.
- **Decide** → if it's a choice you're committing to, write it up in [`decisions/`](./decisions).
- **Archive** → move to [`archive/`](./archive) if it's superseded but worth keeping.
- **Delete** → if it's noise.

Empty inbox = reviewed brain.

---

## Where things live

| Folder | Holds | Source of truth for |
| --- | --- | --- |
| [`inbox/`](./inbox) | Raw, unsorted capture | nothing — it's a staging area |
| [`strategy/`](./strategy) | Vision, positioning, customers, model, GTM, risks, governance, Sapilon synergy | **what we're building and why** |
| [`product/`](./product) | Value prop, use-cases, personas, idea drafts | **what the product is** |
| [`market/`](./market) | Competitor deep-dives, the matrix, observations | **the landscape** |
| [`pricing/`](./pricing) | Current model, assumptions, experiments | **how we charge** |
| [`decisions/`](./decisions) | Lightweight decision log (dated, numbered) | **why we chose X** |
| [`research/`](./research) | Raw notes, links, founder questions | reference |
| [`templates/`](./templates) | Reusable doc skeletons (one-pager, etc.) | reuse |
| [`archive/`](./archive) | Superseded / rejected, kept for history | history |

## Conventions

- **Markdown for prose, YAML for data.** Anything rendered as a table or list elsewhere (competitor matrix, pricing assumptions) is YAML so it has one structured source.
- **`_TEMPLATE.md`** in a folder = copy-me starter; never edit it as content.
- **Dates in filenames** for time-stamped things (`inbox/`, `decisions/`, `archive/` snapshots): `YYYY-MM-DD-slug`.
- Keep each file about **one thing**. If a file grows two topics, split it.

> Full historical plan: [`archive/otopic-business-plan-v1-2026-08-11.md`](./archive/otopic-business-plan-v1-2026-08-11.md) — the monolith this KB was split from (originally `otopic/assets/docs/business-plan.md`).
# otopic-business
