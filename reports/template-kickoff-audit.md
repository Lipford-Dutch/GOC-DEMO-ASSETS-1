# Template Kickoff Audit

## Current State

The repository started with only a README and license. It did not yet provide
the reusable scaffolding expected from an organization template.

## Gaps Found

- No GitHub Actions baseline
- No issue templates
- No pull request template
- No CodeQL, Dependency Review, Scorecard, or Pages workflow
- No security policy
- No contribution or governance model
- No documentation site
- No project kickoff checklist
- No reusable ADR, runbook, release, or risk templates
- README included unsafe license-key storage guidance

## Remediation Applied

- Replaced README with product-neutral template guidance.
- Added governance, support, security, contribution, and conduct files.
- Added MkDocs Material documentation structure.
- Added reusable project kickoff templates.
- Added GitHub issue, PR, workflow, Dependabot, and CODEOWNERS scaffolding.
- Added linting and formatting defaults.

## Remaining Manual Setup

- Repository is now configured as `Lipford-Dutch/GOC-Base-Repo-Template`.
- GitHub template mode is enabled.
- Wiki is enabled and seeded with a base operating manual.
- Social preview source and PNG live under `docs/assets/`.
- Replace placeholder CODEOWNERS with real teams.
- Configure branch protection in GitHub settings.
- Enable secret scanning and push protection.
- Enable dependency graph and GitHub Advanced Security where available so
  Dependency Review, CodeQL, and Scorecard can become blocking controls.
