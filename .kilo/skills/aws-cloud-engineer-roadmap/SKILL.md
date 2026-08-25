---
name: aws-cloud-engineer-roadmap
description: Guide for working with the AWS Cloud Engineer roadmap repository. Use when creating or updating roadmap documents, learning paths, role descriptions, or engagement models for the AWS Cloud Engineer committed role program.
---

# AWS Cloud Engineer Roadmap Skill

## When to Use This Skill

Use this skill when:
- Creating or updating roadmap documents
- Modifying learning path content
- Updating role descriptions
- Editing three-party engagement models
- Adding new skills or AWS services to the curriculum
- Restructuring documentation

## Repository Structure

```
docs/
├── index.html                 # GitHub Pages landing page
├── README.md                  # Documentation index
├── 01-role-description.md     # Role responsibilities & expectations
├── 02-roadmap.md              # 20-week learning roadmap
├── 03-learning-path.md        # Week-by-week curriculum
├── 04-quick-start-guide.md    # Daily routine & success metrics
├── 05-resources.md            # Tools, resources, best practices
├── 06-three-party-engagement.md # Employer-Vendor-Associate model
├── 07-staff-augmentation-proposal.md # Executive proposal
└── .nojekyll                  # Disable Jekyll for GitHub Pages
```

## Document Conventions

### Markdown Documents
- Use ATX-style headings (`##`, `###`)
- Keep line length under 120 characters
- Use relative paths for internal links (`./02-roadmap.md`)
- No YAML frontmatter unless specified
- Add "Continue To" section at the end of each document pointing to next relevant docs

### Numbered Documents
- Format: `NN-document-name.md`
- Numbers must be sequential: 01, 02, 03, etc.
- Case-sensitive naming
- Each document should be self-contained but link to related documents

### HTML Landing Page
- Entry file: `docs/index.html`
- Use relative paths for all internal links
- Keep CSS inline in `<style>` blocks
- Ensure responsive design

## Content Guidelines

### Role Description (01)
- Include: Role overview, responsibilities, skills, soft skills, career growth
- Audience: Employers, stakeholders
- Tone: Professional, clear

### Roadmap (02)
- Include: Phases, timelines, skill progression
- Format: Table with Timeline and Focus Area
- Audience: All stakeholders
- Tone: Structured, progressive

### Learning Path (03)
- Include: Detailed weekly curriculum, objectives, deliverables
- Format: Phase > Week > Topics > Deliverables
- Audience: Associate, trainers
- Tone: Instructional, detailed

### Quick Start Guide (04)
- Include: Prerequisites, environment setup, daily routine, project ideas
- Format: Checklist, daily schedule
- Audience: Associate starting the program
- Tone: Encouraging, actionable

### Resources (05)
- Include: Tools, books, courses, communities, best practices
- Format: Categorized lists
- Audience: All stakeholders
- Tone: Reference-oriented

### Three-Party Engagement (06)
- Include: Party definitions, responsibilities, SLA, revenue model
- Format: Sections per party, tables for clarity
- Audience: Employers, vendors
- Tone: Formal, contractual

### Staff Augmentation Proposal (07)
- Include: Executive summary, resource profile, engagement model, pricing
- Format: Business proposal structure
- Audience: Employers, decision-makers
- Tone: Persuasive, professional

## Adding New Content

### New Phase in Roadmap
1. Update `02-roadmap.md` with new phase
2. Update `03-learning-path.md` with detailed content
3. Update `readme.md` timeline table
4. Update `docs/index.html` if needed

### New Skill or Service
1. Add to appropriate phase in `02-roadmap.md`
2. Add detailed coverage in `03-learning-path.md`
3. Add resources in `05-resources.md` if applicable

### New Document
1. Determine sequential number (NN)
2. Create `docs/NN-document-name.md`
3. Update `docs/README.md` index
4. Update `readme.md` document index
5. Add "Continue To" sections in adjacent documents
6. Update `docs/index.html` if it's a primary doc

## Validation Checklist

Before finalizing any document:
- [ ] Internal links use correct relative paths
- [ ] Document follows naming convention
- [ ] "Continue To" section added at end
- [ ] Content is consistent with other documents
- [ ] No broken references
- [ ] Line length under 120 chars (for markdown)
- [ ] Professional tone maintained
