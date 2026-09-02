---
name: nodejs-development
description: Guide for creating Node.js learning content in the aws-cloud-engineer/node-js/ folder. Use when creating or updating Node.js tutorials, exercises, projects, or reference materials for the zero-to-hero learning path.
---

# Node.js Development Skill

## When to Use This Skill

Use this skill when:
- Creating new Node.js learning documents
- Updating existing Node.js tutorials
- Adding exercises or projects
- Creating reference materials for Node.js concepts
- Working in the `aws-cloud-engineer/node-js/` directory

## Repository Structure

```
aws-cloud-engineer/node-js/
├── README.md                           # Main index and learning path overview
├── programiz-reference.md             # Cross-reference to Programiz JavaScript tutorials
├── pending-tasks.md                    # Track remaining documents to create
├── 01-variables-and-data-types.md      # Phase 1: JavaScript foundations
├── 02-functions-and-scope.md
├── 03-arrays-and-objects.md
├── 04-async-await-promises.md
├── 05-es6-features.md
├── 06-dom-manipulation.md             # (planned)
├── 07-nodejs-introduction.md          # Phase 2: Node.js basics
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

Each learning document should follow this structure:

1. **Title** (`# Topic Name`)
2. **Overview** - Brief description of what this document covers
3. **Topics Covered** - List of subtopics
4. **Content Sections** - Detailed explanations with code examples
5. **Hands-on Exercises** - Practical exercises with solutions
6. **Knowledge Check** - Review questions
7. **Next Steps** - Links to subsequent documents
8. **Additional Resources** - External links (Programiz, YouTube, etc.)

## Content Guidelines

### Code Examples
- Use JavaScript (compatible with Node.js LTS)
- Include comments explaining key concepts
- Show both synchronous and asynchronous approaches where relevant
- Include error handling patterns

### Exercises
- Always provide solution code
- Include 2-3 exercises per document
- Vary difficulty levels

### Knowledge Checks
- Include 4-5 multiple-choice or short-answer questions
- Answers should be derivable from the document content

## Reference Resources

### Primary References
- [Programiz JavaScript Tutorials](https://www.programiz.com/javascript) — Map topics using `programiz-reference.md`
- [Node.js Deep Dive Playlist](https://www.youtube.com/watch?v=pN6jk0uUrD8&list=PLxnjbfm5MCHFbRlyVCAqpJFdIzPN_IPID)

### Quick Start Resources
- [JavaScript Basics in 1 Hour - Mosh](https://www.youtube.com/watch?v=W6DUe7Pgp8A)
- [Node.js Tutorial for Beginners - Mosh](https://www.youtube.com/watch?v=TlB2W5UPEWU)

## Adding New Content

### New Phase Document
1. Follow numbering convention (NN-topic-name.md)
2. Follow the document format template
3. Add "Continue To" section linking to next related docs
4. Update README.md with new document reference
5. Update pending-tasks.md to mark completed item
6. Commit with: `docs: add NN-topic-name.md`

### New Exercise
1. Create in `exercises/` folder if needed
2. Reference the exercise in relevant learning documents
3. Include clear problem statement and solution

### New Project
1. Create in `projects/` folder
2. Reference the project in relevant phase
3. Include project description, requirements, and solution outline

## Validation Checklist

Before finalizing any document:
- [ ] Follows the document format template
- [ ] Code examples are valid and runnable
- [ ] Exercises include solutions
- [ ] Knowledge check questions are answerable
- [ ] Links use relative paths
- [ ] Numbered correctly per the README roadmap
- [ ] "Continue To" section added
- [ ] Cross-references to programiz-reference.md updated if relevant
