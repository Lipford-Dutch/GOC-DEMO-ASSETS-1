# Release Governance

## Versioning

Use semantic versioning when the project publishes artifacts:

- `MAJOR`: incompatible changes
- `MINOR`: backward-compatible features
- `PATCH`: backward-compatible fixes
- prerelease labels for alpha, beta, and release candidates

## Release Checklist

Use `templates/release-checklist.md` for every release.

## Required Evidence

- passing CI
- updated documentation
- known limitations
- rollback instructions
- security findings disposition
- release notes

## Promotion

Promote through environments in order:

1. development
2. staging
3. production

Production promotion should be gated by reviewers.
