---
name: aws-cloud-engineer-roadmap
description: Guide for creating/updating roadmap docs, learning paths, role descriptions, engagement models in the AWS Cloud Engineer committed role program.
---

# AWS Cloud Engineer Roadmap Skill

## When to Use
- Creating/updating roadmap documents
- Modifying learning path content
- Updating role descriptions
- Editing three-party engagement models
- Adding AWS services to curriculum
- Restructuring documentation

## Doc Structure

```
docs/
├── index.html                 # Pages landing page
├── README.md                  # Docs index
├── .nojekyll                  # Disable Jekyll
├── 01-role-description.md
├── 02-roadmap.md
├── 03-learning-path.md
├── 04-quick-start-guide.md
├── 05-resources.md
├── 06-three-party-engagement.md
└── 07-staff-augmentation-proposal.md
```

## Conventions

- Markdown: ATX headings, ≤120 chars, relative paths
- Docs: `NN-name.md`, case-sensitive, sequential
- HTML: `docs/index.html`, inline CSS, relative links
- Commits: `feat:`, `fix:`, `docs:`, `chore:`
- Add "Continue To" at end of each doc

## Doc Content Guidelines

| Doc | Content | Audience | Tone |
|-----|---------|----------|------|
| 01 | Role overview, responsibilities, skills, career growth | Employers | Professional |
| 02 | Phases, timelines, skill progression | All | Structured |
| 03 | Weekly curriculum, objectives, deliverables | Associates | Instructional |
| 04 | Prerequisites, setup, daily routine, projects | New learners | Encouraging |
| 05 | Tools, books, courses, communities, best practices | All | Reference |
| 06 | Party definitions, responsibilities, SLA, revenue | Employers/Vendors | Formal |
| 07 | Exec summary, resource profile, engagement, pricing | Decision-makers | Persuasive |

## New Document Workflow

1. Sequential number (NN) based on existing files
2. Create `docs/NN-document-name.md`
3. Update `docs/README.md`
4. Update `readme.md` document index
5. Add "Continue To" sections
6. Commit: `docs: add NN-document-name.md`

## Validation Checklist

- [ ] Relative paths correct
- [ ] Naming convention followed
- [ ] "Continue To" section added
- [ ] No broken references
- [ ] ≤120 char lines
- [ ] Professional tone
