---
name: nodejs-development
description: Guide for creating Node.js learning content in aws-cloud-engineer/node-js/. Use when creating or updating Node.js tutorials, exercises, projects, or reference materials.
---

# Node.js Development Skill

## When to Use
- Creating/updating Node.js learning documents
- Adding exercises or projects
- Working in `aws-cloud-engineer/node-js/`

## Folder Structure

```
aws-cloud-engineer/node-js/
├── README.md                           # Index & learning path overview
├── programiz-reference.md             # Programiz JS tutorials mapping
├── pending-tasks.md                    # Remaining documents
├── 01-variables-and-data-types.md
├── 02-functions-and-scope.md
├── 03-arrays-and-objects.md
├── 04-async-await-promises.md
├── 05-es6-features.md
├── 07-nodejs-introduction.md
├── 08-npm-and-package-management.md   # (planned)
├── 09-file-system-module.md            # (planned)
├── 10-http-server.md                   # (planned)
├── 11-streams-and-buffers.md          # (planned)
├── 12-error-handling.md               # (planned)
└── projects/                          # (planned)
    ├── todo-app.md
    ├── file-api.md
    ├── blog-api.md
    ├── ecommerce-backend.md
    └── capstone-api.md
```

## Document Format

1. `# Title`
2. Overview
3. Topics Covered
4. Content sections with code examples
5. Hands-on Exercises (with solutions)
6. Knowledge Check (4-5 questions)
7. Next Steps (links)
8. Additional Resources

## Content Guidelines

- **Code**: JavaScript compatible with Node.js LTS, with comments
- **Exercises**: Always include solutions, 2-3 per document
- **References**: [Programiz JS](https://www.programiz.com/javascript), [Node.js Deep Dive](https://www.youtube.com/watch?v=pN6jk0uUrD8&list=PLxnjbfm5MCHFbRlyVCAqpJFdIzPN_IPID)

## New Content Workflow

1. Number document (NN-topic-name.md)
2. Follow format template
3. Add "Continue To" section
4. Update README.md and pending-tasks.md
5. Commit: `docs: add NN-topic-name.md`

## Validation Checklist

- [ ] Follows format template
- [ ] Code examples valid
- [ ] Exercises have solutions
- [ ] Knowledge check answerable
- [ ] Relative paths
- [ ] Correct numbering
- [ ] "Continue To" added
- [ ] programiz-reference.md updated if relevant
