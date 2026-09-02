# Project Memory

## Current State
- Repository: aws-cloud-engineer-road-map
- Branch: main
- Last updated: 2026-08-25
- Status: Active development

## Key Decisions
- Publishing source: `/docs` folder on `main` branch
- Landing page: `docs/index.html`
- Documentation format: Numbered markdown files (01-07)
- GitHub Pages: Uses `.nojekyll` to bypass Jekyll processing
- Agent system: Kilo Code with AGENTS.md, skills, memory, and tasks

## Document Structure
### Root docs/ (GitHub Pages)
- 01-role-description.md
- 02-roadmap.md
- 03-learning-path.md
- 04-quick-start-guide.md
- 05-resources.md
- 06-three-party-engagement.md
- 07-staff-augmentation-proposal.md

### aws-cloud-engineer/node-js/ (Learning Path)
- README.md
- programiz-reference.md
- pending-tasks.md
- 01-05: Phase 1 JavaScript Fundamentals (complete)
- 07: Phase 2 Node.js Basics (in progress)
- 06, 08-12, 13-38: Not yet created (see pending-tasks.md)

## Repository Structure (Updated)
```
.
├── AGENTS.md
├── readme.md
├── docs/
│   ├── index.html
│   ├── README.md
│   ├── .nojekyll
│   └── 01-07-*.md
├── .github/workflows/pages.yml
├── .kilo/
│   ├── skills/
│   │   ├── aws-cloud-engineer-roadmap/SKILL.md
│   │   └── nodejs-development/SKILL.md
│   ├── memory/project-memory.md
│   ├── tasks/tasks.md
│   └── kilo.json
├── .devcontainer/devcontainer.json
├── aws-services/
│   └── 79 service directories
├── aws-cloud-engineer/
│   └── node-js/ (learning path)
├── aws-developer/
├── aws-serverless/
├── node-js/
├── angular/
└── react/
```

## Recent Changes
- Added AGENTS.md for AI agent guidance
- Added .kilo/skills/ for agent skills
- Added .kilo/skills/nodejs-development/SKILL.md
- Added .github/workflows/pages.yml for GitHub Pages deployment
- Fixed readme.md formatting for better readability
- Removed duplicate docs/readme.md that caused case-sensitivity issues
- Added comprehensive AWS service directories under aws-services/
- Added role-specific directories (aws-developer/, aws-serverless/, aws-cloud-engineer/)
- Created Node.js learning path (Phase 1-2 complete, remaining in pending-tasks.md)
- Added devcontainer.json with Node.js, JDK, Python, AWS CLI, Kilo AI
- Created programiz-reference.md mapping Programiz tutorials to learning phases

## Known Issues
- GitHub Pages must be manually enabled in repository settings
- Branch source must be set to `main` and folder to `/docs`
- Some Node.js learning docs reference YouTube playlist for deep dives

## Known Issues
- GitHub Pages must be manually enabled in repository settings
- Branch source must be set to `main` and folder to `/docs`

## Stakeholders
- Employer/Client: Reviews role description and engagement model
- Associate/Engineer: Follows learning path and quick start guide
- Vendor/Training Company: Manages engagement and provides expert support
