# Generals of Chaos Golden Config Demo

This repository contains synthetic, non-production multi-vendor configuration templates for the Nautobot demonstration environment. It intentionally contains no credentials, routable addresses, or production configuration.

The Nautobot Golden Config application uses:

- `templates/` for strict Jinja intended-configuration rendering.
- `intended/` for representative rendered examples.
- `backups/` for representative observed configurations with deliberate drift.

Deployment is disabled in the Nautobot application configuration. Compliance, remediation planning, and change previews remain enabled for safe zero-touch demonstrations.
