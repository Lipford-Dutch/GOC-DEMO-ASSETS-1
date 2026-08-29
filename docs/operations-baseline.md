# Operations Baseline

## Minimum Operational Artifacts

- runbook
- rollback procedure
- backup and restore notes, if data exists
- alerting expectations
- support path
- release checklist
- known failure modes

## Runbook Sections

Use `templates/runbook.md` and include:

- service overview
- dependencies
- normal operation
- incident triage
- recovery
- validation
- escalation

## Production Readiness

Before production, confirm:

- configuration is environment-driven
- secrets are externally managed
- logs are useful and do not expose secrets
- dependency scans are reviewed
- rollback path is tested
- ownership is documented
