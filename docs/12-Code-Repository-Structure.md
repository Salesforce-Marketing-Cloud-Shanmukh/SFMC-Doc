Code Repository Structure
=========================

Branches
--------
- main: production-ready docs and assets.
- develop: integration branch for approved features.
- feature/*: scoped to a specific change with ticket reference.

Conventions
-----------
- Semantic commits; keep CHANGELOG updated per environment.
- Store automation SQL/queries and DE DDL alongside documentation.

CI/CD (Optional)
----------------
- Lint Markdown, validate JSON manifests, broken-link checks.
- GitHub Actions for PR checks and artifact packaging.


