# Business Model

Four tiers serving two distinct motions — hosted SaaS for individuals and the SME wedge, PAYG BYOC for regulated/enterprise (see [`../decisions/0006-four-tier-pricing-free-without-ai.md`](../decisions/0006-four-tier-pricing-free-without-ai.md)).

| Tier | Price | For | Includes |
| --- | --- | --- | --- |
| **Free** | €0 | Team trials, client-side stakeholders, individuals | Full collaboration, all core features, **no AI** — one-time **€1–3 trial AI credit per user** |
| **Standard** | €10–15 / month | One person | AI included, all core features |
| **Teams** | €10–15 / user / month | SME teams (~5–50 people) | AI for the whole team, multiple workspaces, client-branded views, priority support |
| **Enterprise** | Pay-as-you-go (AWS + AI + sub) | Regulated industries, enterprise | BYOC deployment in client's AWS org, SLA, dedicated onboarding |

## Design principles

- **Upgrade triggers are built into the product** — using up the trial AI credit is the natural moment to convert Free → Standard or Teams.
- **Free has no recurring AI** — a one-time €1–3 credit per user lets every user feel the differentiator while keeping Free's AI cost capped.
- **Two pricing motions, not one** — hosted subscription for SME teams, PAYG for enterprise. Forcing one model onto both segments is a named risk (see [`./risks.md`](./risks.md)).
- **Client-side stakeholders stay free** — they are the expansion surface (clients bring Otopic into their own orgs), not a revenue line.
- **Enterprise procurement enters at Enterprise** via Sapilon-delivered engagements — services revenue funds the product while the client becomes a reference logo.

Pricing detail and open questions: [`../pricing/current-model.md`](../pricing/current-model.md).
