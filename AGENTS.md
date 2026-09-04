# AGENTS.md

AWS Cloud Engineer committed-role program repo. Primary artifact is documentation; there is no app runtime, test suite, or build step beyond GitHub Pages deployment.

## What This Repo Is Now

- 33-week learning roadmap for a fresher with no programming background.
- Four parallel tracks from Week 1: Fullstack, Git/IDE/CI-CD, Agile/Architecture, AWS Cloud.
- `docs/` is the GitHub Pages source. `docs/index.html` is the entry point.
- `aws-serverless-developer/` is a standalone 16-week specialized track with its own README and Mermaid diagrams.
- `roadmap-files/CloudEngineer-RoadMap-EntryToMidLevel.md` is the long-form single-file roadmap.

## Conventions

- Markdown: ATX headings, ≤120 chars, relative paths.
- Docs: `NN-name.md` numbering in `docs/` is sequential; case-sensitive.
- Commits: Conventional (`feat:`, `fix:`, `docs:`, `chore:`).
- Mermaid: use `Lambda Edge` instead of `Lambda@Edge`; GitHub’s renderer rejects `@` in node IDs.
- `.nojekyll` must exist in `docs/`; Pages deploy uses the `./docs` artifact path.

## GitHub Pages

- Workflow: `.github/workflows/pages.yml`
- Trigger: push to `main` touching `docs/**`, `readme.md`, or `AGENTS.md`.
- Live site: https://cloudshare360.github.io/aws-cloud-engineer-road-map/
- If Pages content is stale, check workflow run permissions and artifact path `./docs`.

## Kilo Config

- `.kilo/kilo.json`: mode `code`, model `kilo/kilo-auto/free`, skills/memory/tasks enabled.
- Skills: `.kilo/skills/aws-cloud-engineer-roadmap/SKILL.md`, `.kilo/skills/nodejs-development/SKILL.md`
- Memory: `.kilo/memory/`
- Tasks: `.kilo/tasks/`

## Editing Rules

- Do not rename or remove `docs/index.html` or `docs/.nojekyll`.
- When adding a doc, update `docs/README.md`, `readme.md`, and add a “Continue To” section.
- When changing roadmap structure, keep `roadmap-files/CloudEngineer-RoadMap.md` untouched; use `CloudEngineer-RoadMap-EntryToMidLevel.md` for the current curriculum.
- `aws-serverless-developer/` content is independent; do not merge its diagrams into `docs/` unless asked.

## Validation

- No automated tests or linters are configured.
- Before pushing, verify: relative links resolve, headings ≤120 chars, Mermaid syntax avoids `@` in IDs, and `docs/.nojekyll` exists.
