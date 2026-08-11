# Governance — Architecture & Customization Discipline

How we keep one product core while delivering client customizations through Sapilon.

## Isolation model

Otopic is built as **microservices with an isolated customization layer**. Sapilon-delivered customizations live as:

- separate web apps on the core API, or
- custom APIs on the shared database

— **never as forks of core.**

## The 3-client promotion rubric

A custom feature is promoted into Otopic core **only when 3+ clients have requested it independently.**

This rubric exists to prevent the product from being shaped by the loudest client. It is the governance answer to the "one client warps the core" risk in [`./risks.md`](./risks.md).

## Text-first data model

The other standing architectural constraint — structured, minimal text as the source of truth — is recorded as [`../decisions/0001-text-first-data-model.md`](../decisions/0001-text-first-data-model.md).
