# Value Proposition

**Otopic is an AI-native project brain that lives in your cloud** — the workspace for SME teams that need to plan, collaborate with clients, and let AI handle the management overhead, without sending their data to multi-tenant SaaS.

## The core unit: the Topic

A **Topic** is a durable container that holds notes, chat, tasks, decisions, and AI context in one place. Every Topic remembers its own context and history; AI uses that memory to:

- draft updates,
- surface what's stalled,
- answer "where are we on this?" — without anyone writing a status report.

## The three-way promise

Existing tools force a trade-off. Otopic delivers all three:

1. **Simple** — mobile-first, three-tap actions, no setup overhead. An SME team is productive on day one, without an admin or a rollout project.
2. **AI-native** — AI is how work gets organized, not a chatbot on the side. Every note, decision, and task is a first-class input to the AI.
3. **Sovereign** — deployable into the client's own AWS organization. Data never leaves their boundary; compliance becomes architectural, not contractual.

## Why text-first matters to the buyer

Otopic stores work as structured, human-readable text rather than opaque rich-text blobs or visual state. This is not an aesthetic choice:

- **AI reliability** — plain, structured data is what AI models parse accurately. A decision recorded as a short paragraph is one AI can quote, summarize, and link later; a decision buried in a comment thread on a color-coded card is not.
- **Longevity** — plain-text content is portable, diff-able, and survives tooling changes. Readable in ten years without a renderer.

The UI can be rich; the storage layer stays minimal. Full rationale: [`../decisions/0001-text-first-data-model.md`](../decisions/0001-text-first-data-model.md).

## Use-cases

- [`use-cases/client-collaboration.md`](./use-cases/client-collaboration.md) — the SME wedge
- [`use-cases/remote-work.md`](./use-cases/remote-work.md) — the distributed-team operating model
