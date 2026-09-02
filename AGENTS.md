# AGENTS.md

AWS Cloud Engineer Committed Role Program — 20-week training placing a mid-level AWS Cloud Engineer (6 YOE) with technical expert support layer.

## Repository Structure

```
.
├── readme.md                    # Root index
├── docs/
│   ├── index.html               # GitHub Pages landing
│   ├── README.md                # Docs index
│   ├── .nojekyll                # Disable Jekyll
│   └── 01-07-*.md              # Numbered docs
├── .kilo/
│   ├── skills/
│   │   ├── aws-cloud-engineer-roadmap/SKILL.md
│   │   └── nodejs-development/SKILL.md
│   ├── memory/                 # project.md, environment.md, corrections.md, project-memory.md
│   ├── tasks/tasks.md
│   └── kilo.json
├── .devcontainer/devcontainer.json
├── .github/workflows/pages.yml
├── aws-services/               # 79 service dirs
├── aws-cloud-engineer/node-js/ # Node.js learning path
├── aws-developer/
├── aws-serverless/
├── node-js/
├── angular/
└── react/
```

## Conventions

- **Markdown**: ATX headings, ≤120 char lines, relative paths
- **Docs**: `NN-name.md` format, case-sensitive
- **Commits**: Conventional (`feat:`, `fix:`, `docs:`, `chore:`)
- **Pages**: `/docs` folder, `index.html` entry, `.nojekyll` required

## Agent System

- **Skills**: `.kilo/skills/` — load relevant before tasks
- **Memory**: `.kilo/memory/` — update after significant changes
- **Tasks**: `.kilo/tasks/` — predefined workflows

## Environment

```bash
KILO_MODE=code
KILO_MODEL=kilo/kilo-auto/free
```

Devcontainer tools: Node.js LTS, Python, Java, AWS CLI, Kilo CLI (`@kilocode/cli`)
