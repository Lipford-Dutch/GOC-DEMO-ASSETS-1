# GOC-Base-Repo-Template

GOC-Base-Repo-Template is the Lipford-Dutch project kickoff template for new
repositories. It packages the Generals of Chaos baseline operating model,
documentation standards, GitHub automation, triage discipline, security posture,
and release governance that every new codebase should inherit before
product-specific code lands.

The template is intentionally product-neutral. It does not contain application
runtime code, secrets, vendor-specific credentials, or project-specific metrics.

## What This Template Provides

- Repository governance: contribution, security, support, code of conduct, and
  decision-record guidance.
- GitHub operations: issue templates, pull request template, Dependabot,
  Dependency Review, CodeQL, Scorecard, Pages deployment, and documentation CI.
- Documentation system: MkDocs Material structure with kickoff, standards,
  security, release, operations, and General Triaging Chaos playbooks.
- Project readiness assets: ADR, runbook, release checklist, security exception,
  and operational readiness templates.
- Quality defaults: editor settings, Git attributes, markdown/yaml linting, and
  pre-commit hooks.
- Social and launch assets: reusable social preview artwork in
  `docs/assets/social-preview.png` and `docs/assets/social-preview.svg`.

## Kickoff Flow

1. Create a new repository from this template.
2. Replace placeholder ownership in `CODEOWNERS`, `SECURITY.md`, and
   `docs/ownership.md`.
3. Enable GitHub Pages from GitHub Actions.
4. Enable repository security features:
   - Dependabot alerts and security updates
   - Secret scanning and push protection
   - Code scanning
   - Branch protections for `main`
5. Fill out the kickoff checklist in `docs/kickoff-checklist.md`.
6. Create the first ADR from `templates/adr.md`.
7. Open the first product PR with the included pull request template.

## Repository Layout

```text
.
|-- .github/                 # GitHub workflows, templates, and governance
|-- docs/                    # MkDocs source documentation
|-- templates/               # Reusable project artifacts
|-- reports/                 # Audit and readiness reports
|-- mkdocs.yml               # Documentation site configuration
|-- SECURITY.md              # Vulnerability reporting policy
|-- CONTRIBUTING.md          # Contribution and review standards
|-- GOVERNANCE.md            # Ownership and decision model
|-- SUPPORT.md               # Support and escalation expectations
|-- AGENTS.md                # AI agent operating instructions
```

## General Triaging Chaos Operating Model

This template keeps chaos useful by making work visible, classifiable, and
reviewable:

- Capture ambiguity as issues, ADRs, or risks instead of burying it in chat.
- Treat CI as the minimum bar, not the final review.
- Keep repo automation boring, repeatable, and least-privileged.
- Prefer small, reversible changes with explicit acceptance criteria.
- Document the operational path before production traffic exists.

## Local Documentation Preview

```bash
python -m pip install -r requirements-docs.txt
mkdocs serve
```

Build the static documentation site:

```bash
mkdocs build --strict
```

## Social Preview

Use `docs/assets/social-preview.png` as the repository Social Preview image in
GitHub settings. The editable source lives at `docs/assets/social-preview.svg`.
Keep the preview generic so repositories created from this template can reuse or
adapt it without leaking project-specific context.

## Template Boundaries

This repository should stay generic. Do not add:

- production secrets, license keys, or encrypted credentials
- application-specific business logic
- customer data or environment-specific configuration
- tool output that cannot be reused by future repositories
- large binaries or installable executables

Use `docs/examples.md` for generic examples and move product-specific content to
the repository created from this template.
