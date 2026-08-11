# Pricing — Current Model

**Model: three tiers, two motions.** Hosted subscription (Free/Pro) for the freelancer wedge; pay-as-you-go (Sovereign) for regulated/enterprise. Rationale in [`../decisions/0002-three-tier-two-motion-pricing.md`](../decisions/0002-three-tier-two-motion-pricing.md); assumptions in [`./assumptions.yaml`](./assumptions.yaml).

| Tier | Price | For | Includes |
| --- | --- | --- | --- |
| **Free** | €0 | Individuals, freelancers, small teams | Full collaboration, all core features, **30–50 AI actions/month** |
| **Pro** | €10–15 / user / month | Active freelancers, growing teams | Unlimited AI, multiple workspaces, client-branded views, priority support |
| **Sovereign** | Pay-as-you-go: AWS + AI + subscription (+ labor when needed) | Regulated industries, enterprise | BYOC deployment in client's AWS org, SLA, dedicated onboarding |

## How each motion converts

- **Free → Pro:** the upgrade trigger is built into the product — hitting the monthly AI-action quota is the natural conversion moment. Free *includes* AI so the differentiator is felt on day one.
- **Sovereign:** enterprise procurement enters via Sapilon-delivered engagements. Pricing aligns with Sapilon's PAYG model (AI credits + AWS pass-through + subscription + labor) — see [`../strategy/sapilon-synergy.md`](../strategy/sapilon-synergy.md).

## Still open

- Exact Pro price point within the €10–15 band.
- Free-tier AI quota (30 vs. 50 actions/month) and what counts as one "AI action."
- Sovereign PAYG composition: AI-credit markup, AWS pass-through vs. bundled tiers, minimum subscription floor.
- Whether client-side (external stakeholder) seats are ever billable — current lean: no, they are the viral surface.
