# 0002 — Three-tier pricing serving two distinct motions

- **Date:** 2026-08-11
- **Status:** accepted

## Context

Otopic serves two segments with incompatible buying behavior: freelancers/small teams (self-serve, price-sensitive, viral) and regulated/enterprise (procurement-driven, compliance-blocked, BYOC). A single pricing model would mismatch one of them — a named risk in [`../strategy/risks.md`](../strategy/risks.md).

## Decision

Three tiers, two motions:

- **Free (€0)** — full collaboration, all core features, 30–50 AI actions/month. AI is *included* so every user experiences the differentiator on day one.
- **Pro (€10–15/user/month)** — unlimited AI, multiple workspaces, client-branded views, priority support.
- **Sovereign (PAYG: AWS + AI + subscription)** — BYOC in the client's AWS org, SLA, dedicated onboarding; sold through Sapilon engagements.

The Free → Pro upgrade trigger is built into the product: hitting the AI quota.

## Consequences

- Two billing systems to maintain (subscription + metered PAYG), aligned with Sapilon's PAYG model for Sovereign.
- Free tier carries real AI cost — the quota is a marketing spend, sized in [`../pricing/assumptions.yaml`](../pricing/assumptions.yaml).
- Rules out seat-billing external client stakeholders (they are the viral surface).
- Open: exact Pro price point, quota size, Sovereign PAYG composition — tracked in [`../pricing/current-model.md`](../pricing/current-model.md).
