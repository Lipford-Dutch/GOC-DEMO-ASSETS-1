# Security Policy

## Supported Use

This repository is a template. Security issues usually fall into one of these
categories:

- unsafe workflow permissions
- missing security controls
- secret-handling mistakes
- vulnerable template dependencies
- documentation that encourages unsafe practices

## Reporting a Vulnerability

Open a private vulnerability report in GitHub Security Advisories when available.
If private reporting is unavailable, contact the repository owner directly and do
not disclose exploit details in a public issue.

## Baseline Controls

Repositories created from this template should enable:

- Dependabot alerts and security updates
- Dependency Review on pull requests
- CodeQL or equivalent static analysis
- secret scanning and push protection
- branch protection on `main`
- required pull request reviews
- least-privilege GitHub Actions permissions

## Secret Handling

Do not store secrets, license keys, tokens, certificates, private keys, or
customer data in this repository. Use environment-scoped secrets in the target
repository or an approved secrets manager.

## Risk Exceptions

Use `templates/security-exception.md` for documented risk acceptance. Every
exception should include an owner, expiration date, mitigation, and detection
method.
