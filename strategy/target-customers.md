# Target Customers

Two segments, two motions — an SME wedge and a regulated premium. Freelancers are explicitly **not** a launch target (see [`../decisions/0003-sme-teams-first-target.md`](../decisions/0003-sme-teams-first-target.md)).

## Primary — SME teams (~5–50 people)

**Sharpest sub-segment: client-facing services** — agencies, consultancies, studios, professional services. They feel all three pains at once: fragmented tools, management overhead nobody has capacity for, and client communication scattered across email/WhatsApp/docs.

**What Otopic gives them:** every project is a Topic with a note, a chat, and an AI that drafts updates, surfaces stalls, and keeps clients informed — the PM overhead a 5–50 person team can't staff.

**Why they're first:**
- They map exactly to Sapilon's engagement pipeline — Phase 1 references *are* SME teams.
- They buy seats in batches with real budget; "AI writes the status updates" has calculable ROI for a team lead.
- Professional-services SMEs (law, accounting) are the bridge to the regulated premium segment — same buyer, earlier and smaller.

**Expansion motion:** every SME project exposes client-side stakeholders to Otopic; those clients bring it into their own organizations. Team-to-team, via the work itself.

**Motion:** hosted SaaS (Free trial → Teams per-seat), seeded through Sapilon engagements.

## Premium — Regulated & enterprise teams

**Who:** legal, healthcare, biotech, financial services, and enterprises with strict data policies.

**Pain:** currently locked out of modern AI collaboration tools entirely — the data cannot sit in a third-party multi-tenant cloud.

**What Otopic gives them:** BYOC deployment into their own AWS organization. Compliance becomes architectural. Distributed enterprises can deploy per-region for multi-jurisdiction data residency while sharing one project brain.

**Motion:** top-down, sold through Sapilon engagements as the Enterprise tier (see [`./sapilon-synergy.md`](./sapilon-synergy.md)).

## Later — Freelancers & solo operators

Self-serve bottom-of-funnel once the product exists anyway: the Free tier serves them, and some grow into teams. Not a launch target — no marketing spend, no roadmap items driven by this segment before Phase 2 is established.
