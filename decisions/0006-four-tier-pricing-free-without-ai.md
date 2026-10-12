# 0006 — Four tiers; Free without AI beyond a trial credit

- **Date:** 2026-10-12
- **Status:** accepted — supersedes the tier list in [`./0002-three-tier-two-motion-pricing.md`](./0002-three-tier-two-motion-pricing.md) (the two-motion split stands)

## Context

0002 put AI on Free (30–50 actions/month) and had one paid hosted tier, Pro, for teams. That leaves no plan for a single person who wants AI without buying into a team product, and it makes the Free tier carry an open-ended monthly AI cost.

## Decision

Four tiers, still two motions:

- **Free (€0)** — full collaboration, all core features, **no AI** apart from a one-time **€1–3 trial AI credit per user**.
- **Standard (€10–15/month)** — AI included, for **one person**.
- **Teams (€10–15/user/month)** — AI for the whole team, multiple workspaces, client-branded views, priority support. The old Pro, renamed.
- **Enterprise (PAYG: AWS + AI + subscription)** — BYOC in the client's AWS org, SLA, dedicated onboarding. The old Sovereign, renamed; "sovereign" stays the word for the deployment, not the plan.

The upgrade trigger moves from "hit the monthly quota" to "used up the trial credit".

## Consequences

- Free's AI cost is now capped per user (€1–3 once), not recurring — the quota is no longer a standing marketing spend.
- Reverses the `free-includes-ai` assumption: Free users feel the AI only through the trial credit. Risk to watch — a Free user who never spends the credit never sees the differentiator.
- Client-side stakeholders stay free on every plan; whether their questions draw on the host's AI is unchanged (host pool).
- Open, tracked in [`../pricing/current-model.md`](../pricing/current-model.md): exact trial credit, Standard and Teams price points (both carry the old Pro band for now), whether Teams per seat sits above Standard.
