# 0001 — Text-first data model (the AI-readability constraint)

- **Date:** 2026-08-11
- **Status:** accepted

## Context

Modern collaboration tools store work as rich-text blobs, nested boards, and visual state optimized for human scanning. AI agents parse these unreliably — a decision buried in a comment thread attached to a color-coded card is invisible to an LLM. Otopic's core differentiator is AI that reasons over the work itself.

## Decision

Every entity in Otopic (notes, tasks, decisions, updates) is stored as **structured, minimal, human-readable text** — no proprietary binary formats, no deeply nested visual state, no layout metadata baked into content. The UI can be rich; **visual presentation is a read layer on top of durable text, never the source of truth.**

## Consequences

- **AI reliability** — LLMs tokenize and reason over text naturally; every note, decision, and task becomes a first-class AI input the model can quote, summarize, and link to later context.
- **Longevity** — plain-text content is portable, diff-able, survives tooling changes, and is still readable in ten years without a renderer.
- Rules out block-tree/rich-text storage architectures, even if they'd make some UI features easier.
- Constrains every future feature: if a feature's state can't be represented as structured text, it needs a different design.
