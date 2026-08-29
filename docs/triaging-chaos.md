# General Triaging Chaos

General Triaging Chaos is a disciplined way to move fast without hiding risk.

## Principles

- Make uncertainty visible.
- Classify before fixing.
- Keep changes reversible.
- Capture decisions once.
- Automate the boring checks.
- Escalate security and release blockers early.

## Triage Classes

| Class | Meaning | Action |
| --- | --- | --- |
| P0 | Release or production blocker | Stop and fix immediately |
| P1 | Should not ship without disposition | Fix or document risk acceptance |
| P2 | Important improvement | Schedule before next milestone |
| P3 | Nice-to-have | Backlog |

## Issue Labels

Recommended labels:

- `type:bug`
- `type:feature`
- `type:docs`
- `type:security`
- `type:operations`
- `type:ci-cd`
- `priority:p0`
- `priority:p1`
- `priority:p2`
- `priority:p3`

## Triage Loop

1. Capture the issue.
2. Assign type and priority.
3. Identify owner and acceptance criteria.
4. Link validation commands.
5. Close only with evidence.
