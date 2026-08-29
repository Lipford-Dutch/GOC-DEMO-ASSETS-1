# AGENTS.md

These instructions apply to automated coding agents working in repositories
created from this template.

## Operating Principles

- Keep the repository product-neutral until a project explicitly specializes it.
- Do not add secrets, credentials, customer data, or private environment values.
- Prefer small, reviewable changes with tests or validation commands.
- Preserve repository hygiene: documentation, CI, security, and release metadata
  should evolve with code.
- Use conventional commits for generated commit messages.
- When adding automation, use least-privilege GitHub token permissions.
- When adding docs, keep `mkdocs build --strict` passing.

## Validation Baseline

Run the applicable checks before opening a pull request:

```bash
python -m pip install -r requirements-docs.txt
mkdocs build --strict
```

If pre-commit is installed:

```bash
pre-commit run --all-files
```

## Template Safety Rules

- Do not hardcode organization secrets.
- Do not add repository-specific app names, customer names, production URLs, or
  credentials.
- Do not disable security workflows to make a branch green.
- Document accepted risks in `templates/security-exception.md` format.
