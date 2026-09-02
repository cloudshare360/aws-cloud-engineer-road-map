# Environment Commands

## GitHub Pages
- Deployed via `.github/workflows/pages.yml` (trigger: push to main, source: /docs)
- Verify before push: `docs/index.html` exists, `docs/.nojekyll` exists, relative links valid

## Devcontainer
- VS Code: F1 → "Dev Containers: Reopen in Container"
- GitHub Codespaces: create from main branch

## Validation

```bash
# JSON
python3 -c "import json; json.load(open('path/to/file.json'))"

# YAML
python3 -c "import yaml; yaml.safe_load(open('path/to/file.yml'))"
```

## Git Workflow

```bash
git add -A
git commit -m "feat: |fix: |docs: |chore:"
git push origin main
```

## Paths

| Type | Path |
|------|------|
| Root docs | `docs/` |
| Node.js learning | `aws-cloud-engineer/node-js/` |
| Agent skills | `.kilo/skills/` |
| Agent memory | `.kilo/memory/` |
| Agent tasks | `.kilo/tasks/` |
| Devcontainer | `.devcontainer/devcontainer.json` |
| Pages workflow | `.github/workflows/pages.yml` |

## Devcontainer Tools Installed
Node.js LTS, Python 3, Java JDK, AWS CLI v2, npm, pip, git, GitHub CLI, Kilo Code (extension + CLI)

## Env Variables
`KILO_MODE=code`, `KILO_MODEL=kilo/kilo-auto/free`
