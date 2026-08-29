# Governance

This template defines the starting governance model for new Lipford-Dutch
repositories.

## Ownership

- Repository owner: replace with project owner.
- Technical owner: replace with engineering owner.
- Security owner: replace with security or platform owner.
- Operations owner: replace with SRE or operations owner.

Update `.github/CODEOWNERS` before using this template for production work.

## Decision Records

Use `templates/adr.md` for architecture decisions that affect:

- security posture
- deployment model
- data ownership
- operational reliability
- public API behavior
- long-term maintenance cost

Store project ADRs in `docs/decisions/`.

## Change Control

Use pull requests for all changes. Production-impacting repositories should add
branch protection, required reviews, required checks, and release approval gates.

## Risk Acceptance

Use `templates/security-exception.md` when a vulnerability, control gap, or
operational risk cannot be fixed before release.
