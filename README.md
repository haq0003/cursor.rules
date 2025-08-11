# Cursor Rules Pack — Microservices Clean Code & DevOps Standards

This repository contains a **.cursor rules pack** designed for guiding both developers and AI assistants in producing clean, secure, and maintainable code for **microservices** projects using:

- **Docker** & **Kubernetes**
- **GitHub Actions** for CI/CD
- **Terraform** for Infrastructure as Code
- **TypeScript** (frontend/backend) + optional multi-language support

---

## 📂 Structure

```
.cursor/
  index.mdc                       # Global principles & reading order
  rules/
    00-foundations.mdc             # Definition of Done, gates, branching
    01-roles-and-raci.mdc          # Roles & responsibilities
    02-domain-and-architecture.mdc # DDD, boundaries, versioning
    03-typescript-coding-standards.mdc
    04-error-handling-logging-observability.mdc
    05-api-design-and-versioning.mdc
    06-data-management.mdc
    07-service-communication.mdc
    08-containers-and-docker.mdc
    09-kubernetes.mdc
    10-ci-cd-github-actions.mdc
    10-git-and-reviews.mdc
    11-terraform-iac.mdc
    12-testing-strategy.mdc
    13-security.mdc
    14-release-and-operations.mdc
    15-documentation-and-adrs.mdc
    16-tooling.mdc
```

---

## 🚀 Purpose

These rules aim to:
- Maintain **high code quality** across services and teams.
- Ensure **security-by-default** and **observability-by-default**.
- Keep **domain boundaries clear** and APIs stable.
- Align DevOps, CI/CD, and Infrastructure as Code with best practices.
- Provide **scoped rules** via `globs` so only relevant guidance applies.

---

## 🔍 Key Features

- **Severity Levels**: Each rule is tagged with **MUST**, **SHOULD**, or **MAY**.
- **Unique IDs**: Rules have IDs (e.g., `API-REST-03`) for referencing in PR reviews, ADRs, and checklists.
- **Scoped Globs**: Rules attach only to relevant files to reduce noise.
- **PR Checklist**: Built-in code review checklist in `10-git-and-reviews.mdc`.
- **Tooling Map**: `16-tooling.mdc` links rules to automated lint/test/security tools.

---

## 📌 How to Use

1. **Copy `.cursor/` into your repository root**.
2. Commit the rules so **Cursor AI** automatically applies them during coding.
3. Follow the **reading order** in `index.mdc` to understand the hierarchy.
4. For any exceptions, create an **ADR** in `docs/adr/` explaining context, alternatives, decision, and consequences.

---

## 🛠 Suggested Tooling

- **Formatting**: `.editorconfig`, Prettier
- **Linting**: ESLint (TypeScript strict mode), Commitlint
- **Security**: Dependabot/Snyk, Gitleaks/TruffleHog
- **CI/CD**: GitHub Actions with lint, test, build, SAST, SBOM

---

## 📜 License

MIT License — free to use and adapt.

---

## ✍️ Author Notes

This pack is designed to be **living documentation**: update rules as your stack evolves, and enforce them via automated checks wherever possible.
