# Agent Tasks

## 1. Create New Document
**Purpose**: Add numbered document to docs/

**Steps**:
1. Find next NN number in `docs/`
2. Create `docs/NN-document-name.md`
3. Update `docs/README.md` and root `readme.md` indexes
4. Add "Continue To" sections
5. Commit: `[docs|chore]: add NN-document-name.md`

**Validation**: Naming convention, relative links, "Continue To" added, cross-references updated

## 2. Update Learning Path
**Purpose**: Modify week/phase content in docs/03-learning-path.md

**Steps**:
1. Read 03-learning-path.md and 02-roadmap.md for context
2. Update the relevant week/phase
3. Ensure deliverables are measurable
4. Update root readme.md timeline if changed
5. Commit: `docs: update learning path`

**Validation**: Content aligns with roadmap, consistent deliverables, no broken links

## 3. Add AWS Service
**Purpose**: Add new AWS service to curriculum

**Steps**:
1. Add to appropriate phase in 02-roadmap.md
2. Add coverage in 03-learning-path.md
3. Add to 05-resources.md
4. Update readme.md Training table
5. Commit: `feat: add AWS <service>`

**Validation**: Added to roadmap + learning path + resources

## 4. Publish GitHub Pages
**Purpose**: Deploy documentation to GitHub Pages

**Steps**:
1. Verify docs/index.html exists
2. Verify docs/.nojekyll exists
3. Verify .github/workflows/pages.yml exists
4. Check relative paths in all links
5. Commit + push to main
6. Verify Pages settings (main, /docs)

**Validation**: index.html valid, .nojekyll exists, workflow valid YAML, no 404s

## 5. Review Documents
**Purpose**: Audit all documents for consistency

**Steps**:
1. Read all 7 numbered docs in order
2. Check terminology, formatting, links
3. Verify "Continue To" sections present
4. Update outdated content
5. Commit: `docs: review and update`

**Validation**: Consistent terminology, valid links, complete sections

## 6. Update Agent Configuration
**Purpose**: Sync agent config with project changes

**Steps**:
1. Review AGENTS.md accuracy
2. Update .kilo/skills/ if patterns changed
3. Update .kilo/memory/ with recent changes
4. Commit: `chore: update agent configuration`

**Validation**: AGENTS.md current, skills/memory up-to-date, consistent

## 7. Create Node.js Document
**Purpose**: Add Node.js learning doc to aws-cloud-engineer/node-js/

**Steps**:
1. Find next NN number
2. Create `NN-topic-name.md` with format: Overview → Topics → Content → Exercises → Knowledge Check → Next Steps → Resources
3. Add "Continue To" section
4. Update node-js/README.md and pending-tasks.md
5. Commit: `docs: add NN-topic-name.md`

**Validation**: Format follows template, code valid, exercises have solutions, 4-5 knowledge questions, links relative, cross-refs updated

## 8. Update Node.js Document
**Purpose**: Modify existing Node.js learning document

**Steps**:
1. Read target document
2. Make updates maintaining format
3. Check Phase alignment with README.md
4. Update programiz-reference.md if adding resources
5. Commit: `docs: update NN-topic-name.md`

**Validation**: Format consistent, no broken links, content aligned, references updated
