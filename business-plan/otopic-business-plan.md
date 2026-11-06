# Otopic — One-Page Business Plan

> **The project brain that lives in your cloud** — AI-native collaboration for teams and their clients, with sovereignty by design.

**As of:** 2026-11-06 · **Stage:** Phase 1, internal tool inside Sapilon engagements · **Print:** [`otopic-business-plan.pdf`](./otopic-business-plan.pdf) · **Deck:** [`otopic-business-plan.pptx`](./otopic-business-plan.pptx)

<!-- Derived summary, not a source of truth. When a linked KB file changes, update this page, the PDF and the deck together. -->

## Problem

- **Work context evaporates** between the board, the thread, the doc and the WhatsApp group.
- **SME teams can't staff the overhead** — real coordination and client-communication load, no one free to write status updates.
- **AI is bolted on**, running over boards and rich-text blobs it parses poorly.
- **Regulated teams are locked out** — legal, healthcare and finance can't put their data in someone else's cloud.

## Solution

The **Topic**: one durable home for a piece of work — notes, chat, tasks, decisions and AI context. One **agent**, chat or talk, that **finds, does and answers** ("where are we on Acme?"), sees only what the asker may see, and cites its sources. Deployable into the customer's own AWS (BYOC). Build order: chat (find + answer) → do → talk.

## Why we win

- **Simple + AI-native + sovereign.** No tool has all three; any one is copyable, the combination is the moat.
- **Text-first data model** → accurate, cited answers. Incumbents would have to rebuild their core to match.
- **Our own line, not a replacement:** _"Keep chatting anywhere. Otopic is where your work and its decisions live — and you can ask it anything."_
- **Clients are first-class** — they ask a shared topic themselves, on a free seat.

## Why now

"Ask your workspace" is table stakes in 2026 (Microsoft 365 Copilot, Slack AI, Atlassian Rovo, Notion AI), so the contest moves to _what_ the AI runs over, _where_ it runs and _who_ can ask. Remote and hybrid work is permanent and async context loss is unsolved. Regulated industries are compliance-blocked, not price-sensitive.

## Customers

| Segment | Who | Motion |
| --- | --- | --- |
| **Primary** | SME teams of ~5–50, client-facing services first: agencies, consultancies, studios, professional services | Seeded via Sapilon → Free team trial → Teams |
| **Premium** | Regulated & enterprise: legal, healthcare, biotech, finance | Top-down via Sapilon → Enterprise (BYOC) |
| **Later** | Freelancers & solo operators | Self-serve on Free; no spend, no roadmap pull |

## Business model — four tiers, two motions

| Tier | Price | For | Includes |
| --- | --- | --- | --- |
| **Free** | €0 | Team trials, client-side stakeholders, individuals | All core features; no AI beyond a one-time €1–3 trial credit per user |
| **Standard** | €10–15 / month | One person | AI included |
| **Teams** | €10–15 / user / month | SME teams | Team AI, multiple workspaces, client-branded views, priority support |
| **Enterprise** | PAYG: AWS + AI + subscription (+ labor) | Regulated, enterprise | BYOC in the client's AWS org, SLA, dedicated onboarding |

**Conversion is built in:** the trial credit runs out → Standard or Teams; a second person joins → Teams; Enterprise enters through Sapilon engagements. Only agent _answers_ draw on AI — search and simple commands are free on every tier. Client-side seats are never billed. _Illustrative: a 20-seat Teams account ≈ €2.4–3.6k ARR._

## Go-to-market

1. **Phase 1 — internal tool** (mid-2026 → early 2027, **we are here**): inside every Sapilon engagement, no public marketing; goal **5–10 reference clients**, funded by services.
2. **Phase 2 — standalone product** (2027 → mid-2028): public launch of Free / Standard / Teams; Enterprise packaged through Sapilon; content on AI + project execution feeds both funnels.
3. **Phase 3 — decision point** (mid-2028+): spin out as an independent company or stay Sapilon's flagship. Architecture and brand stay spin-out-ready.

**Growth loop:** every project invites client-side stakeholders for free → they experience Otopic as "how this firm works" → they bring it into their own organizations.

## Operations & funding

One offer, two revenue streams: **Sapilon services + Otopic recurring**. Shared tech core, one content engine, and every engagement ships a customized sovereign Otopic instance — a Sapilon revenue line _and_ an Otopic logo. R&D is funded by a revenue-percentage rule with ring-fenced engineering hours; separate funding and team are a Phase 3 question. Customizations never fork core; a feature joins core only when **3+ clients** ask for it independently.

## Top risks → mitigations

| Risk | Mitigation |
| --- | --- |
| Sapilon emergencies eat Otopic dev time | Ring-fenced hours + revenue-percentage R&D rule |
| Heavy AI users turn margin-negative | Only answers count; fair-use limit; measure AI cost per active user before fixing prices |
| Agent leaks across a sharing boundary | Answers scoped to what the asker can see, tested before launch, always cited |
| "Ask your workspace" is commoditized | Compete on cited answers over text-first topics, AI in the customer's cloud, clients asking topics |
| BYOC operational complexity | Deployment automation (Terraform/CDK) before scaling Enterprise |
| One client warps the core | Isolated customization layer + 3-client promotion rubric |

## Phase 1 must prove (by early 2027)

- **5–10 reference clients** live on Otopic through Sapilon engagements.
- **AI cost per active user and per answer** → sets the Standard / Teams prices and the fair-use limit.
- **Trial-credit behavior** — share of Free users who spend it, and conversion after it runs out.
- **How the agent is used** — answers vs. commands, and talk-mode retention.

**Still open:** exact price points (does a Teams seat sit above Standard?) · trial-credit size · Enterprise PAYG composition · market size — not yet quantified.

---

<sub>Sources: [vision](../strategy/vision.md) · [positioning](../strategy/positioning.md) · [target customers](../strategy/target-customers.md) · [business model](../strategy/business-model.md) · [pricing](../pricing/current-model.md) · [assumptions](../pricing/assumptions.yaml) · [go-to-market](../strategy/go-to-market.md) · [Sapilon synergy](../strategy/sapilon-synergy.md) · [governance](../strategy/governance.md) · [risks](../strategy/risks.md) · [market observations](../market/observations.md) · [agent](../product/agent.md) · decisions [0001](../decisions/0001-text-first-data-model.md)–[0006](../decisions/0006-four-tier-pricing-free-without-ai.md)</sub>
