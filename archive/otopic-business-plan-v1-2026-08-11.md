# Otopic — Business Plan

## 1. Executive Summary

Otopic is an **AI-native project brain that lives in your cloud**. It is the workspace for teams and freelancers who need to plan, collaborate with clients, and let AI handle the management overhead — without sending their data to multi-tenant SaaS.

Where existing tools force a trade-off between simplicity, AI depth, and data sovereignty, Otopic delivers all three. The core unit is the **Topic** — a durable container that holds notes, chat, tasks, decisions, and AI context in one place.

## 2. The Problem

- **Work is fragmented** across calendars, chats, docs, and task boards. Context evaporates between them.
- **AI is bolted on**, not embedded. Most tools added a chatbot; none made AI the way work gets organized.
- **Sovereignty is incompatible with modern tools.** Regulated industries (legal, healthcare, finance, enterprise) cannot use Notion, Asana, or ClickUp because the data sits in someone else's cloud.
- **Modern tools are opaque to AI.** Nested boards, rich-text blobs, and visual kanban layouts are optimized for human scanning — not machine parsing. AI agents struggle to extract meaning from them reliably.

No tool today is simple, AI-native, *and* sovereign. That is Otopic's market.

## 3. Solution & Positioning

**Otopic is the project brain that lives in your cloud — AI-native collaboration for teams and their clients, with sovereignty by design.**

- **Project brain** — every Topic remembers its own context, decisions, and history. AI uses that memory to draft updates, surface what's stalled, and answer "where are we on this?" without anyone writing a status report.
- **Lives in your cloud** — deployable to the client's own AWS organization. Data never leaves their boundary. Compliance becomes architectural, not contractual.
- **Simple by default** — mobile-first, three-tap actions, no setup overhead. Built for freelancers as much as for enterprise teams.
- **Minimal and text-first by design** — Otopic stores work as structured, human-readable text rather than opaque rich-text blobs or visual state. This is not an aesthetic choice: plain, structured data is what AI models parse accurately and reliably. Every note, decision, and task is a first-class input to the AI — not an afterthought.

## 4. Differentiation

|                          | Notion | Asana / ClickUp | Jira  | Self-hosted | **Otopic** |
| ------------------------ | ------ | --------------- | ----- | ----------- | ---------- |
| AI-native                | Partial | No             | No    | No          | **Yes**    |
| Simple & mobile-first    | Partial | No             | No    | No          | **Yes**    |
| Data sovereignty (BYOC)  | No     | No              | No    | Yes (clunky) | **Yes**   |
| Built-in client collab   | No     | Partial         | No    | No          | **Yes**    |

The defensible moat is the **combination**. Any single attribute is replicable; all three together is not.

## 5. Target Market

**Wedge — Freelancers & small teams (2–15 people).** Their pain is the client-collaboration gap: scattered updates over email, WhatsApp, and shared docs. Otopic gives them a shared workspace where every project has a note, a chat, and an AI that keeps clients informed. **Viral motion:** one freelancer brings Otopic to 3–5 client engagements.

**Premium — Regulated & enterprise teams.** Legal, healthcare, biotech, financial services, and enterprises with strict data policies. They are currently locked out of modern AI collaboration tools. Otopic's BYOC deployment unlocks them.

## 6. Business Model

Three tiers serving two distinct motions:

| Tier           | Price                          | For                                  | Includes                                                                  |
| -------------- | ------------------------------ | ------------------------------------ | ------------------------------------------------------------------------- |
| **Free**       | €0                             | Individuals, freelancers, small teams | Full collaboration, all core features, **30–50 AI actions/month**         |
| **Pro**        | €10–15 / user / month          | Active freelancers, growing teams     | Unlimited AI, multiple workspaces, client-branded views, priority support |
| **Sovereign**  | Pay-as-you-go (AWS + AI + sub) | Regulated industries, enterprise      | BYOC deployment in client's AWS org, SLA, dedicated onboarding            |

**Upgrade triggers** are built into the product — hitting the AI quota is the natural moment to convert from Free to Pro. Enterprise procurement enters at Sovereign via Sapilon-delivered engagements.

## 7. Go-to-Market — Three Phases

**Phase 1 (months 0–9): Internal tool.** Otopic is used inside every Sapilon engagement. No public marketing. The goal is real usage data and 5–10 reference clients funded by services revenue.

**Phase 2 (months 9–24): Standalone product.** Public launch with Free + Pro tiers. Sovereign tier sold through Sapilon as a packaged offering. Content marketing on AI + project execution drives both businesses.

**Phase 3 (year 2+): Decision point.** Otopic either spins out as an independent product company (with separate funding and team) or remains Sapilon's flagship product. The architecture and brand keep both options open.

## 8. Sapilon Synergy

Otopic and Sapilon (AI software services) share three layers:

- **Technical core** — every Sapilon AI engineering capability serves Otopic and vice versa.
- **Go-to-market** — one thought-leadership engine drives both demand funnels.
- **Reference clients** — Sapilon engagements ship a customized, sovereign Otopic instance as part of the deliverable. The client becomes both a Sapilon revenue line *and* an Otopic logo.

The framing is one offer with two revenue streams: **services (Sapilon) + recurring product (Otopic)**. Pricing models align around pay-as-you-go (AI credits + AWS pass-through + subscription + labor when needed) for the Sovereign tier.

## 9. Architecture & Customization Discipline

Otopic is built as **microservices with an isolated customization layer**. Sapilon-delivered customizations live as separate web apps on the core API or custom APIs on the shared database — never as forks of core.

A custom feature is **promoted into Otopic core only when 3+ clients have requested it independently**. This rubric exists to prevent the product from being shaped by the loudest client.

**Text-first data model — the AI-readability constraint.** Every entity in Otopic (notes, tasks, decisions, updates) is stored as structured, minimal text — no proprietary binary formats, no deeply nested visual state, no layout metadata baked into content. This constraint serves two purposes:

1. **AI reliability** — LLMs tokenize and reason over text naturally. A decision recorded as a short paragraph with a clear outcome is one an AI can quote, summarize, and link to later context. A decision buried in a comment thread attached to a color-coded card is not.
2. **Longevity** — plain-text content is portable, diff-able, and survives tooling changes. It is still readable in ten years without a renderer.

The UI can be rich; the storage layer stays minimal. Visual presentation is a read layer on top of durable text — never the source of truth.

## 10. Key Risks & Mitigations

| Risk                                                  | Mitigation                                                                                                            |
| ----------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Otopic dev time stolen by Sapilon emergencies         | Ring-fenced engineering hours per week, protected from reallocation. A revenue-percentage rule funds Otopic R&D.      |
| One client's needs warping the core product           | Microservice isolation + the 3-client promotion rubric.                                                               |
| Pricing model mismatch between segments               | Two pricing motions, not one: hosted SaaS (Free/Pro) for freelancers, PAYG (Sovereign) for enterprise.                |
| BYOC operational complexity                           | Heavy investment in deployment automation (Terraform/CDK) before scaling Sovereign tier.                              |
| Free users diluting the AI-native positioning         | Free tier *includes* AI (rate-limited), so every user experiences the differentiator on day one.                      |

## 11. Remote Work Enablement

The shift to distributed and hybrid work is permanent, not cyclical. Otopic is architected from the ground up for teams that are never in the same room.

**Why existing tools fail distributed teams:**
- Status updates require manual effort — someone has to write them, someone has to read them. Context falls through the cracks across time zones.
- Chat-first tools (Slack, Teams) produce ephemeral knowledge. Decisions made in a thread are invisible 48 hours later.
- Async collaboration breaks down when the "project brain" is a combination of a Notion doc, a Jira board, and a WhatsApp group.

**How Otopic addresses this:**

| Challenge | Otopic's answer |
| --------------------------------- | --------------- |
| Async status visibility | AI drafts standing updates from topic activity — no human writes the Monday morning summary |
| Decisions get lost | Every topic maintains a decision log; AI surfaces relevant past decisions when new ones are made |
| Client communication across TZs | Client-facing views in the topic mean external stakeholders self-serve rather than pinging |
| Onboarding remote contractors | A new contributor reads a topic's AI-summarized history and is productive without a call |
| Meeting reduction | When context is always current and searchable, most sync calls become unnecessary |

**Remote-native features on the roadmap:**
- **Async video notes** — record a 60-second context drop inside a topic; AI transcribes, indexes, and links it to relevant tasks
- **Time-zone-aware nudges** — AI surfaces blockers to the right person at a time they are likely to be online
- **Presence-light collaboration** — thread-style replies on tasks and decisions with inline AI synthesis, so threads don't require a live meeting to resolve

**Sovereign deployment amplifies this.** A globally distributed enterprise team can deploy Otopic in a regional AWS zone closest to each office cluster, meet data-residency requirements in multiple jurisdictions simultaneously, and still share a single unified project brain — without routing sensitive data through a third-party SaaS.

Remote work is not a use case Otopic accommodates; it is the primary operating model Otopic was designed for.

## 12. Vision

Otopic is not a task manager. It is **a memory of work, a decision ledger, and a knowledge graph for execution** — running on infrastructure the customer owns.

> *Convert your business actions into data. Let AI make sense of it. Keep the data yours.*