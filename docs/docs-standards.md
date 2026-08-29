# Documentation Standards

## Required Audiences

Write for these audiences:

- new contributor
- maintainer
- security reviewer
- release manager
- operator

## Required Content

Every project should document:

- installation or bootstrap path
- configuration
- local validation
- CI/CD behavior
- security assumptions
- release process
- rollback process
- known limitations

## Style

- Prefer direct, testable instructions.
- Include commands that can be copied into a terminal.
- Keep project-specific tribal knowledge in the repository.
- Use diagrams when they clarify ownership, flow, or deployment.

## Validation

Run:

```bash
mkdocs build --strict
```
