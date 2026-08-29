# Generals of Chaos Nautobot Golden Config Demo

This branch specializes the GOC demo-assets repository for a synthetic,
multi-vendor Nautobot Golden Config demonstration. It contains no production
credentials, routable infrastructure addresses, customer data, or live-device
configuration.

## Demonstration Scope

- Cisco IOS-XE, IOS-XR, and NX-OS style intended configuration.
- Juniper Junos style intended configuration.
- Fortinet FortiOS style intended configuration.
- F5 BIG-IP TMOS style intended configuration.
- Representative observed backups with deliberate drift.
- Intended configurations suitable for compliance and remediation previews.

The Nautobot Golden Config application uses:

- `templates/` for strict Jinja intended-configuration rendering.
- `intended/` for representative rendered examples.
- `backups/` for representative observed configurations with deliberate drift.

Deployment is disabled in Nautobot. Backup, intended configuration,
compliance, remediation planning, and change previews remain enabled so the
environment can demonstrate zero-touch workflows without attempting network
connections to synthetic devices.

## Branch and Repository Model

The canonical assets are published from the
`nautobot-golden-config-demo` branch of `Lipford-Dutch/GOC-DEMO-ASSETS-1`.
Other application demonstrations can use independent branches without sharing
runtime state or configuration history.

## Governance Baseline

This branch inherits the Generals of Chaos repository controls, including:

- contribution, security, support, code-of-conduct, and governance policies;
- issue and pull-request templates;
- Dependabot, dependency review, CodeQL, Scorecard, and documentation CI;
- ADR, runbook, release, security-exception, and operational-readiness templates;
- strict MkDocs, Markdown, YAML, and pre-commit quality defaults.

Use the assets only for demonstration. Never commit credentials, encrypted
secrets, production backups, customer information, or live network endpoints.

## Validation

Render all Jinja templates with strict undefined-variable handling against
representative Nautobot devices. Validate the repository documentation with:

```bash
python -m pip install -r requirements-docs.txt
mkdocs build --strict
```
