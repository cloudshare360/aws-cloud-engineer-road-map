# Project Facts

## Project Name
AWS Cloud Engineer Committed Role Program

## Repository
https://github.com/cloudshare360/aws-cloud-engineer-road-map

## Purpose
A structured 20-week training and placement framework that positions a mid-level AWS Cloud Engineer (6 YOE) into a committed, full-time role backed by a technical expert support layer.

## Repository Type
- Documentation repository (Markdown + HTML)
- Static site (GitHub Pages from /docs folder)
- No build step required for documentation
- Learning materials repository

## Key Technologies
- Documentation: Markdown, HTML5, CSS (inline)
- Hosting: GitHub Pages
- CI/CD: GitHub Actions
- AI Agents: Kilo Code with AGENTS.md, skills, memory, and tasks
- Development: Node.js, VS Code, Codespaces

## Repository Structure
```
.
├── AGENTS.md                      # Root agent instructions
├── readme.md                     # Main index and roadmap
├── docs/                         # GitHub Pages content
│   ├── index.html                # Landing page
│   ├── README.md                 # Docs index
│   ├── .nojekyll                 # Disable Jekyll
│   └── 01-07-*.md               # Numbered docs
├── .kilo/                        # Agent configuration
│   ├── skills/                   # Agent skill files
│   ├── memory/                   # Memory files
│   ├── tasks/                    # Task definitions
│   └── kilo.json                 # Kilo CLI config
├── .devcontainer/                # Codespaces configuration
│   └── devcontainer.json
├── .github/
│   └── workflows/
│       └── pages.yml             # GitHub Pages workflow
├── aws-services/                 # 79 AWS service directories
├── aws-cloud-engineer/           # Role-specific content
│   └── node-js/                  # Node.js learning path
├── aws-developer/                # Developer role resources
├── aws-serverless/               # Serverless resources
├── aws-cloud-engineer/           # Role folder
├── node-js/                      # Frontend/backend folder
├── angular/                      # Frontend/backend folder
└── react/                        # Frontend/backend folder
```

## Key Conventions
- Markdown: ATX headings, 120 char line limit, relative paths for links
- Documents: Numbered format (01-07), case-sensitive naming
- Commit messages: Conventional commits (feat:, fix:, docs:, chore:)
- GitHub Pages: Publish from main branch /docs folder
- Files: index.html as entry point, .nojekyll to disable Jekyll
