# AGENTS.md

AWS Cloud Engineer Committed Role Program — 20-week training placing a mid-level AWS Cloud Engineer (6 YOE) with technical expert support layer.

## Repository Structure

```
.
├── readme.md                    # Root index
├── docs/                        # GitHub Pages (01-07*.md + index.html + README.md)
├── .kilo/                       # Agent config
├── .devcontainer/devcontainer.json
├── .github/workflows/pages.yml
├── aws-cloud-engineer/          # Role root
│   ├── node-js/                 # Node.js learning path
│   ├── angular/                 # Frontend resources
│   ├── react/                   # Frontend resources
│   ├── dev-ops/                 # DevOps learning materials
│   │   ├── ci-cd/               # GitLab, GitHub Actions, Jenkins
│   │   └── iac/                 # CloudFormation, CDK, Terraform, OpenTofu
│   └── aws-services/            # 82 AWS services organized by domain
│       ├── analytics/
│       ├── application-integration/
│       ├── compute/
│       ├── containers/
│       ├── database/
│       ├── developer-tools/
│       ├── iot/
│       ├── machine-learning/
│       ├── management-governance/
│       ├── migration-transfer/
│       ├── networking-content-delivery/
│       ├── security-identity-compliance/
│       ├── serverless-application-repository/
│       └── storage/
```

## Conventions

- Markdown: ATX headings, ≤120 chars, relative paths
- Docs: `NN-name.md` format, case-sensitive
- Commits: Conventional (`feat:`, `fix:`, `docs:`, `chore:`)
- Pages: `/docs` folder, `index.html` entry, `.nojekyll`

## Agent System

- Skills: `.kilo/skills/`
- Memory: `.kilo/memory/`
- Tasks: `.kilo/tasks/`

## Environment

```bash
KILO_MODE=code
KILO_MODEL=kilo/kilo-auto/free
```

Devcontainer: Node.js LTS, Python, Java, AWS CLI, Kilo CLI
