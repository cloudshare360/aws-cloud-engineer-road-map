# Agent Tasks

## Task: Create New Document

### Description
Create a new numbered document in the docs/ folder following established conventions.

### Steps
1. Determine the next sequential number (NN) by checking existing files
2. Create `docs/NN-document-name.md` with appropriate frontmatter and content
3. Update `docs/README.md` to include the new document
4. Update `readme.md` Document Index table
5. Add "Continue To" section in adjacent documents
6. Update `docs/index.html` if it's a primary document
7. Commit with message: `docs: add NN-document-name.md`

### Validation
- [ ] File follows naming convention `NN-document-name.md`
- [ ] Document is self-contained but links to related docs
- [ ] "Continue To" section added
- [ ] All cross-references updated

---

## Task: Update Learning Path

### Description
Update the learning path content for a specific week or phase.

### Steps
1. Read `docs/03-learning-path.md` to understand current structure
2. Read `docs/02-roadmap.md` to ensure alignment
3. Make updates to the relevant week/phase
4. Ensure deliverables are clear and measurable
5. Update `readme.md` if timeline changes
6. Commit with message: `docs: update learning path for Week NN`

### Validation
- [ ] Content aligns with roadmap
- [ ] Deliverables are specific and measurable
- [ ] Cross-references are updated
- [ ] No broken links

---

## Task: Add New AWS Service

### Description
Add a new AWS service to the curriculum and documentation.

### Steps
1. Add service to appropriate phase in `docs/02-roadmap.md`
2. Add detailed coverage in `docs/03-learning-path.md`
3. Add resources in `docs/05-resources.md`
4. Update `readme.md` Training & Ramp-Up table if needed
5. Update `docs/index.html` if needed
6. Commit with message: `feat: add AWS <service> to curriculum`

### Validation
- [ ] Service added to roadmap
- [ ] Learning content is detailed and practical
- [ ] Resources are accurate and up-to-date
- [ ] Cross-references updated

---

## Task: Publish to GitHub Pages

### Description
Deploy documentation to GitHub Pages.

### Steps
1. Ensure `docs/index.html` exists and is valid
2. Ensure `docs/.nojekyll` exists
3. Ensure `.github/workflows/pages.yml` exists
4. Verify all internal links use relative paths
5. Commit and push to main branch
6. Verify GitHub Pages settings in repository
7. Check deployment status in Actions tab

### Validation
- [ ] `docs/index.html` is present and valid
- [ ] `docs/.nojekyll` exists
- [ ] Workflow file is valid YAML
- [ ] Site is accessible at expected URL
- [ ] No 404 errors in browser console

---

## Task: Review and Update Documents

### Description
Review all documents for consistency, accuracy, and completeness.

### Steps
1. Read all 7 numbered documents in order
2. Check for consistency in terminology and formatting
3. Verify all internal links work correctly
4. Check for broken references or outdated information
5. Ensure "Continue To" sections are present
6. Update any outdated content
7. Commit with message: `docs: review and update documentation`

### Validation
- [ ] All documents reviewed
- [ ] Terminology is consistent
- [ ] All links are valid
- [ ] No outdated information
- [ ] Formatting is consistent

---

## Task: Update Agent Configuration

### Description
Update AGENTS.md, skills, or memory based on project changes.

### Steps
1. Review current `AGENTS.md` for accuracy
2. Update project structure if files were added/removed
3. Update skills in `.kilo/skills/` if new patterns emerged
4. Update memory in `.kilo/memory/` with recent changes
5. Commit with message: `chore: update agent configuration`

### Validation
- [ ] AGENTS.md reflects current project state
- [ ] Skills are up-to-date
- [ ] Memory is current
- [ ] All agent files are consistent

---

## Task: Create Node.js Learning Document

### Description
Create a new Node.js learning document in the `aws-cloud-engineer/node-js/` folder following the established format.

### Steps
1. Determine the next sequential number (NN) by checking existing files in `aws-cloud-engineer/node-js/`
2. Create `aws-cloud-engineer/node-js/NN-topic-name.md` with the document format:
   - Overview, Topics Covered, Content Sections, Hands-on Exercises, Knowledge Check, Next Steps
3. Add "Continue To" section at the end linking to related documents
4. Update `aws-cloud-engineer/node-js/README.md` to include the new document
5. Update `aws-cloud-engineer/node-js/pending-tasks.md` to mark item as completed
6. Commit with message: `docs: add NN-topic-name.md`

### Validation
- [ ] File follows naming convention `NN-topic-name.md`
- [ ] Document follows the learning path format template
- [ ] Code examples are valid JavaScript
- [ ] Exercises include solutions
- [ ] Knowledge check has 4-5 questions
- [ ] "Continue To" section added
- [ ] All cross-references updated
- [ ] README.md updated
- [ ] pending-tasks.md updated

---

## Task: Update Existing Node.js Document

### Description
Update an existing Node.js learning document with new content, corrections, or improvements.

### Steps
1. Read the target document in `aws-cloud-engineer/node-js/`
2. Make content updates while maintaining format consistency
3. Check the corresponding Phase number in README.md
4. Update any references in related documents
5. If adding new resources, update programiz-reference.md
6. Commit with message: `docs: update NN-topic-name.md`

### Validation
- [ ] Changes maintain document format
- [ ] No broken links introduced
- [ ] Content aligns with roadmap and learning path
- [ ] programiz-reference.md updated if needed
