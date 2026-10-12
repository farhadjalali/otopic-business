# 0005 — One agent is how users meet Otopic's AI

- **Date:** 2026-10-12
- **Status:** accepted

## Context

The business model assumes AI everywhere: AI-native is differentiator #1, the Free → Pro trigger is the AI-action quota, Pro sells unlimited AI ([`./0002-three-tier-two-motion-pricing.md`](./0002-three-tier-two-motion-pricing.md)). The product has no AI yet, so there is no upgrade trigger and nothing that proves the claim. Phase 1 reference clients need to experience it before the Phase 2 launch.

Users need one obvious place to use the AI — and it must not become the "chatbot on the side" the vision rules out ([`../strategy/vision.md`](../strategy/vision.md), principle 2).

## Decision

Build **the Otopic agent**: one entry point, always in reach — a floating button bottom-right on mobile, the first item in the nav bar on desktop — that users **talk to (voice) or chat with**. It does three jobs over the user's own data:

1. **Find** — search topics, notes, chats, schedules and contacts.
2. **Do** — act through a defined list of actions (create a topic, add a note, schedule, share, …).
3. **Answer** — questions grounded in existing topics: notes, chats, schedules, sharing.

Product description: [`../product/agent.md`](../product/agent.md).

### Guardrails — what keeps it AI-native, not a bolted-on chatbot

- **First, not hidden.** It is the first thing in the navigation, not a help widget.
- **It acts, not just talks.** Over time, anything a user can do in a few taps they can ask the agent to do; its action list grows with the product.
- **It only knows what the asker may see.** Search and answers never cross a sharing boundary.
- **It cites.** Every answer links to the note, message or schedule it came from.
- **It confirms before changing what others see** — sharing, sending a message, deleting.
- **It isn't the whole AI story.** The vision's proactive AI — drafted status updates, surfacing stalls — still comes. The agent is the front door, not the house.

## Consequences

- The agent is where the AI quota is felt, so "what counts as an AI action" must be answered against it — proposal in [`../pricing/current-model.md`](../pricing/current-model.md).
- Talk (voice) carries a per-minute running cost that chat doesn't — tracked in [`../pricing/assumptions.yaml`](../pricing/assumptions.yaml).
- Sovereign deployments run the agent's AI inside the customer's own cloud. An agent capability that only works by sending data to an outside AI service breaks the Sovereign promise.
- New risks recorded in [`../strategy/risks.md`](../strategy/risks.md): cross-boundary leaks, unlimited-AI cost, commoditised workspace Q&A, voice novelty, AI leaving the boundary.
- **Sequencing (recommended, open):** chat with Find + Answer first (the vision's "where are we on this?"), then Do, then Talk on the same agent — one agent with two ways in, never two features.
