---
name: agent-ops-mini-sprint
description: 'Evidence-first operating workflow for production incident triage, PR risk review, deploy smoke checks, and handoff notes from public or sanitized context.'
---

# Agent Ops Mini-Sprint

Use this skill when a user needs a small, bounded operations sprint with AI coding agents:

- production bug or incident triage
- PR risk review
- deploy smoke checks
- AI-generated code cleanup scoping
- implementation handoff from public or sanitized evidence

## Operating Rules

- Work from evidence before naming a cause.
- Separate observed facts, assumptions, and unknowns.
- Use absolute timestamps when investigating incidents or deploy windows.
- Split the path by layer: frontend, API, auth, database, queue/cache, worker/webhook, provider, runtime, and deploy.
- Prefer read-only checks before mutations, restarts, rollbacks, or manual data edits.
- Never request or expose secrets, tokens, private customer data, payment details, or credentials.
- Keep the first deliverable small enough to verify in one review cycle.

## Incident Triage Output

Return:

1. current read: what is happening, what is not proven, whether it is ongoing
2. timeline: report time, deploys, logs, alerts, admin actions, provider events
3. layer checks: fastest read-only proof for each plausible layer
4. likely causes: ranked by evidence strength with why each may be wrong
5. safe next action: smallest check or patch that increases certainty or reduces impact

## PR Risk Review Output

Lead with findings, not summary.

For each finding include:

- severity
- file or route evidence
- failure mode
- missing test or verification
- minimal fix direction

Prioritize correctness, security, data loss, auth, money-path behavior, race conditions, and deploy regressions over style.

## Deploy Smoke Output

Return:

- target environment and deploy identifier
- health endpoints or user flows checked
- runtime/log checks
- rollback watchpoints
- before/after evidence
- handoff note for the next operator

## Paid Sprint Intake

If the user wants a human-reviewed mini-sprint, ask them to open a sanitized request:

https://mysubb01.github.io/agent-ops-command-pack-teaser/order.html

Public issues are only for sanitized context, scope, budget, and acceptance criteria. Payment links, invoices, and private handoffs happen outside public issues.
