# Repository Standards

## Required Files

Every child repository should keep:

- `README.md`
- `LICENSE`
- `SECURITY.md`
- `CONTRIBUTING.md`
- `SUPPORT.md`
- `GOVERNANCE.md`
- `.github/CODEOWNERS`
- `.github/pull_request_template.md`
- issue templates
- documentation source under `docs/`

## Automation Standards

- Use least-privilege workflow permissions.
- Pin action versions to major versions at minimum.
- Avoid broad write permissions unless a workflow publishes artifacts.
- Keep release workflows separate from validation workflows.
- Prefer reusable scripts over copy-pasted inline logic when workflows grow.

## Documentation Standards

- Documentation must build from a clean checkout.
- Operational procedures must include validation and rollback steps.
- Known limitations must be explicit.
- Architecture decisions belong in ADRs.

## Template Hygiene

Do not add product-specific implementation details to this template. Put examples
in `docs/examples.md` only when they are reusable across projects.
