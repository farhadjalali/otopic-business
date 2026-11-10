# Business Plan

The KB compiled into things you can hand to someone. **Derived, not a source of truth:** every claim here comes from `strategy/`, `product/`, `market/`, `pricing/` and `decisions/`. If it disagrees with them, they win.

| File | What | Use it for |
| --- | --- | --- |
| [`otopic-business-plan.md`](./otopic-business-plan.md) | One-page plan, linked back to its sources | Reading and editing; the text the other two are built from |
| [`otopic-business-plan.pdf`](./otopic-business-plan.pdf) | The same page as a print-ready A4 | Sending, printing |
| [`otopic-business-plan.pptx`](./otopic-business-plan.pptx) | 18-slide deck with speaker notes | Presenting to partners, clients, investors |

## Keeping it current

- When a source file changes in a way the plan reflects (a tier, a price, a phase, a segment), update the `.md` first, then regenerate the PDF and the deck in the same commit.
- When the plan is superseded as a whole, move all three to `archive/` with a date (`archive/otopic-business-plan-v2-YYYY-MM-DD.*`) and start the next version here.
- Known gaps, called out on the page and in the deck: no market sizing and no financial projections yet. The ARR figures are seat arithmetic on the placeholder price band, not a forecast.
