# 0004 — Otopic has its own line; it is not a Slack, Teams or Jira replacement

- **Date:** 2026-10-12
- **Status:** accepted

## Context

Remote, hybrid and team work is a founding reason for Otopic ([`../product/use-cases/remote-work.md`](../product/use-cases/remote-work.md)). The tools those teams live in today are a messenger (Slack, Microsoft Teams) for talk and a tracker (Jira or a board) for work. Pitching Otopic as "the modern, intelligent replacement for Jira, Slack and Teams" is tempting, but:

- **Chat is the hardest switch.** A messenger only works when everyone moves — the whole company and its outside partners. Teams sits inside the Microsoft 365 world most SMEs already run.
- **Jira isn't our buyer's tool.** Client-facing service SMEs ([`./0003-sme-teams-first-target.md`](./0003-sme-teams-first-target.md)) run on email, WhatsApp, Teams and light boards — not Jira.
- **A replacement pitch invites a feature-parity fight** — calls, huddles, app directories, workflow engines — that a simple product loses by design.
- **"Ask your workspace" is no longer unique.** Microsoft 365 Copilot, Slack AI, Atlassian Rovo and Notion AI all answer questions across a workspace. Otopic can't win on "has AI"; it wins on what the AI works over and where it runs.

## Decision

Otopic has **its own line: simplicity and AI-native design** — the place where a remote or hybrid team's work and decisions live, and where anyone on the work can ask it anything.

- We replace the **patchwork** (a board + a thread + a doc + a WhatsApp group), not any one tool. Teams keep chatting wherever they chat; Otopic is where work is remembered.
- Simplicity + AI-native is the line for the SME motion. Sovereignty stays the third leg, carried by the Sovereign tier for the regulated segment.
- Working line: _"Keep chatting anywhere. Otopic is where your work and its decisions live — and you can ask it anything."_

## Consequences

- Positioning, the competitor matrix and market observations now name Slack and Microsoft Teams as where remote teams live, and incumbent workspace AI is on the watch list.
- Chat attached to work (topic, contact and group chats) stays core, but we don't chase messenger parity. A chat request that only makes sense for a general-purpose messenger fails this test.
- Marketing never says "replaces Slack / Teams / Jira". Comparison content contrasts _where context ends up_, not feature lists.
- The AI-native claim has to be visible in the product, not just the copy — see [`./0005-one-agent-talk-or-chat.md`](./0005-one-agent-talk-or-chat.md).
