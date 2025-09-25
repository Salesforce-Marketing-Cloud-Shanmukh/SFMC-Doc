Migration & Deployment Playbooks
================================

General Process
---------------
1. Branch and PR: feature branch per change; peer review required.
2. Package: use Package Manager for journeys, automations, and assets when available.
3. Manual Steps: document exact steps for items unsupported by packages.
4. Validation: smoke tests, link validation, personalization checks.
5. Rollback: archived previous versions, disable/stop journeys safely.

Checklists
----------
- Pre-deploy: dependencies, data availability, triggered send keys, API creds.
- Post-deploy: send classification, tracking, data retention, alerts.

Samples
-------
- package.manifest.json (example placeholder for supported assets)
- SQL scripts for DE creation with indexes and data retention policies.


