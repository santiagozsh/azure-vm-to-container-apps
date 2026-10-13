# azure-vm-to-container-apps

Monorepo for a simulated migration: a real estate agency's Legacy System (single hand-built Azure VM) moved to Azure Container Apps, managed PostgreSQL, and Blob Storage, with Terraform and GitHub Actions (OIDC). Everything in this repo is written in English.

## Layout

- `apps/web`: Next.js (Catalog + Admin Panel)
- `apps/api`: FastAPI
- `infra/`: Terraform (`bootstrap/`, shared modules, per-environment roots)
- `legacy/`: hand-provisioning of the Legacy System VM and data migration scripts
- `docs/`: migration narrative, ADRs (`docs/adr/`), diagrams, runbooks
- `.github/workflows/`: CI/CD

## Agent skills

### Issue tracker

Issues and wayfinder maps live in GitHub Issues (`santiagozsh/azure-vm-to-container-apps`), via the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Default five canonical labels (`needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`). See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: `GLOSSARY.md` and `docs/adr/` at the repo root. See `docs/agents/domain.md`.
