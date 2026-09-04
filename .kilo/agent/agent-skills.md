# Agent Skills

Agent skills for the AWS Cloud Engineer roadmap project.

## Skills Directory

```
.kilo/skills/
├── aws-cloud-engineer-roadmap/SKILL.md
└── nodejs-development/SKILL.md
```

## Available Skills

- **aws-cloud-engineer-roadmap**: Guide for creating/updating roadmap docs, learning paths, role descriptions, engagement models
- **nodejs-development**: Guide for creating Node.js learning content in aws-cloud-engineer/node-js/

## Usage

Skills are auto-loaded by Kilo based on the task context. When working on roadmap documentation, the `aws-cloud-engineer-roadmap` skill is active. When working on Node.js content, the `nodejs-development` skill is active.

## Adding New Skills

1. Create a new directory under `.kilo/skills/`
2. Add a `SKILL.md` with frontmatter and instructions
3. Update `kilo.json` if needed
