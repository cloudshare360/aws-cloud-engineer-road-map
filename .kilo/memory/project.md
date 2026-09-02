# Project Facts

## Project
AWS Cloud Engineer Committed Role Program — 20-week training placing a mid-level AWS Cloud Engineer (6 YOE) with technical expert support layer.

## Repository
https://github.com/cloudshare360/aws-cloud-engineer-road-map

## Type
Documentation repo + static site (GitHub Pages) + learning materials

## Tech Stack
- Docs: Markdown, HTML5, inline CSS
- Hosting: GitHub Pages (/docs folder)
- CI/CD: GitHub Actions
- AI: Kilo Code (AGENTS.md, skills, memory, tasks)
- Dev: Node.js LTS, VS Code, Codespaces

## Structure
```
.
├── readme.md                    # Root index
├── docs/                        # GitHub Pages (01-07*.md + index.html + README.md)
├── .kilo/                       # Agent config (skills, memory, tasks, kilo.json)
├── .devcontainer/devcontainer.json
├── .github/workflows/pages.yml
├── aws-cloud-engineer/
│   ├── node-js/                 # Node.js learning path
│   ├── angular/                 # Frontend resources
│   ├── react/                   # Frontend resources
│   └── aws-services/            # 79 service dirs
```

## Conventions
- Markdown: ATX headings, ≤120 chars, relative paths
- Docs: `NN-name.md` format, case-sensitive
- Commits: Conventional (`feat:`, `fix:`, `docs:`, `chore:`)
- Pages: `/docs` folder, `index.html` entry, `.nojekyll`
