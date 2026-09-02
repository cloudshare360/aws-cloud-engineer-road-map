# AGENTS.md

## Project Overview

AWS Cloud Engineer Committed Role Program — a structured 20-week training and placement framework that positions a mid-level AWS Cloud Engineer (6 YOE) into a committed, full-time role backed by a technical expert support layer.

## Purpose of This File

This file provides instructions for AI coding agents (GitHub Copilot, Kilo Code, Cursor, Windsurf, etc.) working on this repository. It defines the project structure, conventions, and available skills so AI agents can contribute effectively.

## Repository Structure

```
.
├── AGENTS.md                      # AI agent instructions
├── readme.md                     # Root index for stakeholders
├── docs/
│   ├── index.html                # GitHub Pages landing page
│   ├── README.md                 # Documentation index
│   ├── .nojekyll                 # Disable Jekyll for GitHub Pages
│   ├── 01-role-description.md    # Role responsibilities & expectations
│   ├── 02-roadmap.md             # 20-week learning roadmap
│   ├── 03-learning-path.md       # Week-by-week curriculum
│   ├── 04-quick-start-guide.md   # Daily routine & success metrics
│   ├── 05-resources.md           # Tools, resources, best practices
│   ├── 06-three-party-engagement.md # Employer-Vendor-Associate model
│   └── 07-staff-augmentation-proposal.md # Executive proposal
├── .kilo/
│   ├── skills/                   # Agent skills (SKILL.md files)
│   │   ├── aws-cloud-engineer-roadmap/
│   │   │   └── SKILL.md          # Roadmap-specific agent guidance
│   │   └── nodejs-development/
│   │       └── SKILL.md          # Node.js development guidance
│   ├── memory/                   # Agent memory bank
│   │   └── project-memory.md     # Current project state and decisions
│   ├── tasks/                    # Agent task definitions
│   │   └── tasks.md              # Predefined task workflows
│   └── kilo.json                 # Kilo CLI configuration
├── .devcontainer/
│   └── devcontainer.json         # Codespaces configuration
├── .github/
│   └── workflows/
│       └── pages.yml             # GitHub Pages deployment workflow
├── aws-services/                 # 79 AWS service directories
├── aws-cloud-engineer/
│   └── node-js/                  # Node.js zero-to-production learning path
├── aws-developer/                # Developer role resources
├── aws-serverless/               # Serverless engineering resources
├── node-js/                      # Frontend/backend folder
├── angular/                      # Frontend/backend folder
└── react/                        # Frontend/backend folder
```

## Tech Stack

- **Documentation**: Markdown, HTML5
- **Hosting**: GitHub Pages (from `/docs` folder)
- **CI/CD**: GitHub Actions
- **AI Agents**: Kilo Code / GitHub Copilot / Cursor

## Coding Conventions

- **Markdown**: Use ATX-style headings (`##`, `###`), keep line length under 120 chars
- **HTML**: Semantic HTML5, inline CSS in `<style>` blocks for single-file pages
- **Links**: Use relative paths for internal docs (`./02-roadmap.md`)
- **Commit messages**: Conventional commits (`feat:`, `fix:`, `docs:`, `chore:`)
- **Frontmatter**: No YAML frontmatter in markdown docs unless specified

## Document Naming

- All docs use `NN-document-name.md` format (01-07)
- Case-sensitive: `01-role-description.md`, not `01-Role-Description.md`
- Landing page is always `index.html` in the `/docs` root

## GitHub Pages Rules

- Publishing source: `main` branch, `/docs` folder
- Entry file must be `index.html` at the top of `/docs`
- `.nojekyll` must exist in `/docs` to prevent Jekyll from ignoring files starting with `_` or numbered files
- All internal links in `index.html` must use relative paths (`./02-roadmap.md`, not `../docs/02-roadmap.md`)

## Agent Skills

See `.kilo/skills/` for available skills. Agents should load relevant skills before performing tasks.

## Agent Memory

See `.kilo/memory/` for project memory and context. Agents should update memory after significant changes.

## Agent Tasks

See `.kilo/tasks/` for predefined task definitions. Agents can execute or reference these tasks.
