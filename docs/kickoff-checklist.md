# Kickoff Checklist

Use this checklist before the first product code lands.

## Repository Identity

- [ ] Replace placeholder ownership in `.github/CODEOWNERS`.
- [ ] Confirm license selection.
- [ ] Update `README.md` with product purpose and support path.
- [ ] Configure repository description, topics, and homepage URL.
- [ ] Enable GitHub Pages from GitHub Actions.

## Security

- [ ] Enable Dependabot alerts.
- [ ] Enable Dependabot security updates.
- [ ] Enable secret scanning and push protection.
- [ ] Enable CodeQL or equivalent static analysis.
- [ ] Add environment-scoped secrets only after environments exist.
- [ ] Confirm no secrets or license keys are committed.

## Branch Protection

- [ ] Protect `main`.
- [ ] Require pull requests before merge.
- [ ] Require status checks.
- [ ] Require at least one approving review.
- [ ] Dismiss stale approvals when new commits are pushed.
- [ ] Restrict force pushes and deletions.

## Documentation

- [ ] Build docs locally with `mkdocs build --strict`.
- [ ] Create the first ADR in `docs/decisions/`.
- [ ] Complete `docs/project-intake.md`.
- [ ] Complete `docs/ownership.md`.
- [ ] Add project-specific runbooks from `templates/runbook.md`.

## Release Readiness

- [ ] Define versioning policy.
- [ ] Define release branches or tags.
- [ ] Define rollback expectations.
- [ ] Complete the first release checklist from `templates/release-checklist.md`.
- [ ] Confirm package/container artifact strategy, if applicable.
