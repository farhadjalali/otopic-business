# Use-case — Remote Work Enablement

The shift to distributed and hybrid work is permanent, not cyclical. Remote work is not a use case Otopic accommodates; **it is the primary operating model Otopic was designed for.**

**The gap:** remote, hybrid and team work is a huge, permanent need, and there is still no _simple_ tool built for it. Distributed teams assemble a messenger, a tracker and a doc tool, and context falls between them. Otopic doesn't replace any one of them; it is where the work is remembered ([`../../decisions/0004-own-line-not-a-replacement.md`](../../decisions/0004-own-line-not-a-replacement.md)).

## Why existing tools fail distributed teams

- Status updates require manual effort — someone has to write them, someone has to read them. Context falls through the cracks across time zones.
- Chat-first tools (Slack, Teams) produce ephemeral knowledge. Decisions made in a thread are invisible 48 hours later.
- Async collaboration breaks down when the "project brain" is a combination of a Notion doc, a Jira board, and a WhatsApp group.

## How Otopic addresses this

| Challenge                       | Otopic's answer                                                                                                                                |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Async status visibility         | AI drafts standing updates from topic activity — no human writes the Monday morning summary                                                    |
| Decisions get lost              | Every topic maintains a decision log; AI surfaces relevant past decisions when new ones are made                                               |
| Client communication across TZs | Client-facing views in the topic mean external stakeholders self-serve rather than pinging                                                     |
| Onboarding remote contractors   | A new contributor asks the agent to catch them up on a topic and is productive without a call                                                  |
| Meeting reduction               | When context is always current and searchable, most sync calls become unnecessary                                                              |
| Questions across time zones     | Ask the agent instead of waiting for a colleague to wake up — the answer comes from the topic, with its sources ([`../agent.md`](../agent.md)) |
| Capturing on the move           | Talk to the agent — "add to Acme: client approved the colours" — without opening the app's screens                                             |

## Remote-native features on the roadmap

- **Async video notes** — record a 60-second context drop inside a topic; AI transcribes, indexes, and links it to relevant tasks
- **Time-zone-aware nudges** — AI surfaces blockers to the right person at a time they are likely to be online
- **Presence-light collaboration** — thread-style replies on tasks and decisions with inline AI synthesis, so threads don't require a live meeting to resolve

## Sovereign deployment amplifies this

A globally distributed enterprise team can deploy Otopic in a regional AWS zone closest to each office cluster, meet data-residency requirements in multiple jurisdictions simultaneously, and still share a single unified project brain — without routing sensitive data through a third-party SaaS.
