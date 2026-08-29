# CI/CD Baseline

## Validation Workflow

The default CI workflow validates:

- repository required-file presence
- markdown style
- yaml style
- MkDocs strict build

Child repositories should extend CI with language-specific checks:

- lint
- format
- unit tests
- integration tests
- dependency audit
- package or container build

## Release Workflow

Use a separate release workflow for publishing. Release workflows should:

- require protected branches or tags
- use GitHub environments for approvals
- publish immutable artifacts
- attach release notes
- avoid broad token permissions

## Deployment Environments

Recommended environments:

- `development`
- `staging`
- `production`

Production should require reviewers and a wait timer when deployments can affect
users.
