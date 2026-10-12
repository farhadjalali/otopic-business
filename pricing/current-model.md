# Pricing — Current Model

**Model: four tiers, two motions.** Hosted subscription (Free/Standard/Teams) for individuals and the SME wedge; pay-as-you-go (Enterprise) for regulated/enterprise. Rationale in [`../decisions/0006-four-tier-pricing-free-without-ai.md`](../decisions/0006-four-tier-pricing-free-without-ai.md) (tiers) and [`../decisions/0002-three-tier-two-motion-pricing.md`](../decisions/0002-three-tier-two-motion-pricing.md) (two motions); assumptions in [`./assumptions.yaml`](./assumptions.yaml).

| Tier           | Price                                                        | For                                                | Includes                                                                         |
| -------------- | ------------------------------------------------------------ | -------------------------------------------------- | -------------------------------------------------------------------------------- |
| **Free**       | €0                                                           | Team trials, client-side stakeholders, individuals | Full collaboration, all core features, **no AI** — one-time **€1–3 trial AI credit per user** |
| **Standard**   | €10–15 / month                                               | One person                                         | AI included, all core features                                                   |
| **Teams**      | €10–15 / user / month                                        | SME teams (~5–50 people)                           | AI for the whole team, multiple workspaces, client-branded views, priority support |
| **Enterprise** | Pay-as-you-go: AWS + AI + subscription (+ labor when needed) | Regulated industries, enterprise                   | BYOC deployment in client's AWS org, SLA, dedicated onboarding                   |

## How each motion converts

- **Free → Standard / Teams:** the upgrade trigger is built into the product — using up the trial AI credit is the natural conversion moment. The credit is how a Free user feels the differentiator; there is no recurring Free quota.
- **Standard → Teams:** a second person joins and the team wants shared AI, workspaces, and client-branded views.
- **Enterprise:** enterprise procurement enters via Sapilon-delivered engagements. Pricing aligns with Sapilon's PAYG model (AI credits + AWS pass-through + subscription + labor) — see [`../strategy/sapilon-synergy.md`](../strategy/sapilon-synergy.md).

## Still open

- Exact trial credit within €1–3, and whether it is one-time (current lean) or refills.
- Standard and Teams price points — both carry the old Pro band (€10–15) for now; whether a Teams seat should sit above Standard.
- What one AI answer costs against the credit. Carried over from the 2026-10-12 proposal, against the agent's three jobs ([`../product/agent.md`](../product/agent.md)):
  - **Draws on AI:** an _answer_ — a question answered from topic content, a summary, a drafted update.
  - **Always free:** _find_ (search) and simple _do_ commands (create a topic, add a note, set a reminder) — on every tier, including Free after the credit is spent.
  - **Talk** costs more per minute than chat; it draws on the same credit faster.
- Whether Standard and Teams AI need a published fair-use limit — lean: yes.
- Who pays for a client-side stakeholder's questions on a shared topic — lean: the host team's pool (they are its expansion surface), never the client.
- Enterprise PAYG composition: AI-credit markup, AWS pass-through vs. bundled tiers, minimum subscription floor.
- Whether client-side (external stakeholder) seats are ever billable — current lean: no, they are the viral surface.
