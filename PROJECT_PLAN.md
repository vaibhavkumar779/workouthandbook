# PROJECT_PLAN.md

# Fitness Handbooks - Master Project Plan

> Living document. Update this file before implementing major features.

## Vision
Transform the current GitHub Pages fitness handbook into a production-grade, cloud-native, AI-powered fitness platform while **preserving the existing static portal**.

## Current State
- Static HTML/CSS/JS
- GitHub Pages
- LocalStorage
- CSV backup
- Multi-profile dashboards
- Client-side authentication

## Guiding Principles
1. Never break the existing GitHub Pages deployment.
2. Migrate incrementally.
3. Documentation-first.
4. Infrastructure as Code.
5. Security by Design.
6. Test everything.
7. Automate everything.

## Repository Evolution

```
Current
index.html
style.css
*.html
*_data.csv

↓

Future

frontend/
backend/
agents/
data/
infra/
monitoring/
docs/
.github/
```

## Planned Folder Structure

```
frontend/
backend/
agents/
  coach/
  nutrition/
  planner/
  prompts/
  memory/
data/
  csv/
  json/
  migrations/
infra/
  terraform/
  kubernetes/
  helm/
  docker/
monitoring/
docs/
testing/
scripts/
```

## Roadmap

- Phase 0 - Existing Static Portal
- Phase 1 - Documentation
- Phase 2 - Modern Frontend
- Phase 3 - Go Backend
- Phase 4 - PostgreSQL & Redis
- Phase 5 - Authentication
- Phase 6 - Docker
- Phase 7 - Kubernetes
- Phase 8 - GitOps
- Phase 9 - Observability
- Phase 10 - AI Agents
- Phase 11 - Production SaaS

## AI Agents Template

For every new agent document:

- Name
- Purpose
- Inputs
- Outputs
- Memory
- Prompt
- Tools
- Workflow
- Guardrails
- Testing
- Future Improvements

## Feature Template

- Problem
- Requirements
- Design
- API
- UI
- Tests
- Documentation
- Deployment
- Rollback

## Definition of Done

- Documentation updated
- Tests passing
- Security reviewed
- CI green
- README updated
- Changelog updated

# Developer Prompt

Use this prompt whenever implementing features:

> You are contributing to the Fitness Handbooks project.
> Preserve backwards compatibility with the existing GitHub Pages static implementation.
> Prefer Go for backend services, React/Next.js for future frontend, PostgreSQL for persistence, Redis for caching, Docker for containers, Kubernetes for orchestration, Terraform for infrastructure, GitHub Actions for CI/CD, Prometheus/Grafana/Loki/OpenTelemetry for observability, and Agentic AI for intelligent coaching.
> Always update documentation, architecture diagrams, ADRs, tests, and changelog alongside code.
> Do not remove existing functionality unless a migration plan is documented.
