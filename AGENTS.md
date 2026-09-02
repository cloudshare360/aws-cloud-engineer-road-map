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
│   ├── aws-developer/           # Developer role resources
│   ├── aws-serverless/          # Serverless resources
│   └── aws-services/             # 79 AWS service dirs
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
