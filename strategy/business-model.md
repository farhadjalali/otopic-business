# Business Model

Three tiers serving two distinct motions — hosted SaaS for the freelancer wedge, PAYG BYOC for regulated/enterprise.

| Tier | Price | For | Includes |
| --- | --- | --- | --- |
| **Free** | €0 | Individuals, freelancers, small teams | Full collaboration, all core features, **30–50 AI actions/month** |
| **Pro** | €10–15 / user / month | Active freelancers, growing teams | Unlimited AI, multiple workspaces, client-branded views, priority support |
| **Sovereign** | Pay-as-you-go (AWS + AI + sub) | Regulated industries, enterprise | BYOC deployment in client's AWS org, SLA, dedicated onboarding |

## Design principles

- **Upgrade triggers are built into the product** — hitting the AI quota is the natural moment to convert Free → Pro.
- **Free tier includes AI** (rate-limited), so every user experiences the differentiator on day one. Free without AI would dilute the AI-native positioning.
- **Two pricing motions, not one** — hosted subscription for freelancers/teams, PAYG for enterprise. Forcing one model onto both segments is a named risk (see [`./risks.md`](./risks.md)).
- **Enterprise procurement enters at Sovereign** via Sapilon-delivered engagements — services revenue funds the product while the client becomes a reference logo.

Pricing detail and open questions: [`../pricing/current-model.md`](../pricing/current-model.md).
