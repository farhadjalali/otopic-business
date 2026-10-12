# Pricing — Current Model

**Model: three tiers, two motions.** Hosted subscription (Free/Pro) for the SME wedge; pay-as-you-go (Sovereign) for regulated/enterprise. Rationale in [`../decisions/0002-three-tier-two-motion-pricing.md`](../decisions/0002-three-tier-two-motion-pricing.md); assumptions in [`./assumptions.yaml`](./assumptions.yaml).

| Tier          | Price                                                        | For                                                | Includes                                                                  |
| ------------- | ------------------------------------------------------------ | -------------------------------------------------- | ------------------------------------------------------------------------- |
| **Free**      | €0                                                           | Team trials, client-side stakeholders, individuals | Full collaboration, all core features, **30–50 AI actions/month**         |
| **Pro**       | €10–15 / user / month                                        | SME teams (~5–50 people)                           | Unlimited AI, multiple workspaces, client-branded views, priority support |
| **Sovereign** | Pay-as-you-go: AWS + AI + subscription (+ labor when needed) | Regulated industries, enterprise                   | BYOC deployment in client's AWS org, SLA, dedicated onboarding            |

## How each motion converts

- **Free → Pro:** the upgrade trigger is built into the product — hitting the monthly AI-action quota is the natural conversion moment. Free _includes_ AI so the differentiator is felt on day one.
- **Sovereign:** enterprise procurement enters via Sapilon-delivered engagements. Pricing aligns with Sapilon's PAYG model (AI credits + AWS pass-through + subscription + labor) — see [`../strategy/sapilon-synergy.md`](../strategy/sapilon-synergy.md).

## Still open

- Exact Pro price point within the €10–15 band.
- Free-tier AI quota (30 vs. 50 actions/month) and what counts as one "AI action." **Proposal (2026-10-12)**, against the agent's three jobs ([`../product/agent.md`](../product/agent.md)):
  - **Counts:** an _answer_ — a question answered from topic content, a summary, a drafted update.
  - **Free:** _find_ (search) and simple _do_ commands (create a topic, add a note, set a reminder). Charging for these would teach Free users to avoid the agent — the opposite of AI-native.
  - **Talk** costs more per minute than chat. Lean: the same rule (only answers count), plus a monthly talk-minute cap on Free and fair use on Pro.
- Whether Pro's "Unlimited AI" needs a published fair-use limit — lean: yes.
- Who pays for a client-side stakeholder's questions on a shared topic — lean: the host team's pool (they are its expansion surface), never the client.
- Sovereign PAYG composition: AI-credit markup, AWS pass-through vs. bundled tiers, minimum subscription floor.
- Whether client-side (external stakeholder) seats are ever billable — current lean: no, they are the viral surface.
