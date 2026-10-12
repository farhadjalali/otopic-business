# The Otopic agent

The one place users meet Otopic's AI: talk to it or chat with it, and it finds, does and answers. Why and guardrails: [`../decisions/0005-one-agent-talk-or-chat.md`](../decisions/0005-one-agent-talk-or-chat.md).

## Where it lives

- **Mobile** — a floating button, bottom-right, on every screen.
- **Desktop** — the first item in the nav bar.

One tap opens it. It knows where you are: opened from a topic, "add a note here" means that topic.

## Two ways in

- **Chat** — type, read the reply.
- **Talk** — speak and hear the answer back, for hands-busy moments: walking between meetings, driving, on site. The exchange is kept as text, so a spoken request is as findable as a typed one.

Same agent, same abilities, same permissions in both.

## Three jobs

| Job        | Examples                                                                                                                                      | Role in the business                                                      |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| **Find**   | "the topic about the Acme logo" · "where did we talk about the invoice?"                                                                      | Table stakes — every tool searches. Free; never draws on AI credit.   |
| **Do**     | "new topic: Q4 offsite" · "add to Acme: client approved the colours" · "remind me about this Friday at 10" · "share it with the design group" | The zero-tap input method that makes _simple by default_ real.            |
| **Answer** | "where are we on the website?" · "what did we decide about hosting?" · "what's due for Acme this week?" · "draft this week's update for Acme" | The paid hero — the vision's "no one writes a status report again".       |

## First action list

Grouped by what users already do in Otopic:

- **Topics** — create, rename, edit the note, add or tick a step, move to a section, mute, move to trash / restore.
- **Schedules** — set or change a topic's reminder; list what's coming up.
- **Sharing** — share a topic with a contact or group; stop sharing _(always confirms)_.
- **Chats** — post in a topic's chat; message a contact or group _(always confirms before sending)_.
- **Contacts** — add a contact; add someone to a group.

Left out at first: anything without an undo (emptying the trash), account and billing changes.

## What it answers from

Everything the asker can see, and nothing else: topic notes and their change history, steps, schedules, topic / contact / group chats, who a topic is shared with, contacts, file names.

## How each persona uses it

- **Team lead** — "where are we on everything for Acme?" replaces the Monday status round.
- **Account manager** — "draft this week's update for the client" from the topic itself.
- **Client-side stakeholder** — asks a shared topic "where are we?" and gets an answer limited to what's shared with them. Free seat; this is the expansion loop ([`./use-cases/client-collaboration.md`](./use-cases/client-collaboration.md)).
- **Remote contractor** — "catch me up on this topic" instead of an onboarding call ([`./use-cases/remote-work.md`](./use-cases/remote-work.md)).

## Open

- Whose AI pool a client-side stakeholder's question draws on — lean in [`../pricing/current-model.md`](../pricing/current-model.md).
- File contents in answers (not just names) — when.
- Talk-mode languages: teams and their clients don't all speak English.
- Proactive AI (status drafts, stall alerts): delivered _by_ the agent as a message, or in the topic?
- Name and voice: "the agent", or a named persona?
