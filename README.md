# GOC-DEMO-ASSETS-1

Various Generals of Chaos demo assets.

This repository was created from
[GOC-Base-Repo-Template](https://github.com/Lipford-Dutch/GOC-Base-Repo-Template)
on 2026-08-29. It currently holds the template baseline only: the
documentation set under `docs/`, the reusable templates under `templates/`, the
kickoff audit under `reports/`, the GitHub automation under `.github/`, and the
governance files. No demo-specific assets have landed yet.

## What is here today

| Path | Contents |
| --- | --- |
| `docs/` | Template docs (standards, CI/CD, security, operations, release governance) and `docs/assets/social-preview.*` |
| `templates/` | ADR, runbook, release checklist, repo kickoff, operational readiness and security exception templates |
| `reports/template-kickoff-audit.md` | Kickoff audit inherited from the template |
| `mkdocs.yml`, `requirements-docs.txt` | MkDocs configuration for a docs site |

## Adding demo assets

1. Add assets under a top-level folder per demo (for example `demos/<name>/`).
2. Describe each demo in this README with what it shows and where it is used.
3. Keep secrets, customer data and internal hostnames out of this public repo.

## Related

- [GOC-Base-Repo-Template](https://github.com/Lipford-Dutch/GOC-Base-Repo-Template): the kickoff template this repo came from
- [Generals of Chaos](https://cbgoc-cloud.top)

## License

See [LICENSE](LICENSE).
