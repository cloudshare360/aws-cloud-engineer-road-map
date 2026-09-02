# Environment Commands

## Build and Deploy

### GitHub Pages
```bash
# GitHub Pages is deployed via GitHub Actions workflow
# Workflow file: .github/workflows/pages.yml
# Trigger: push to main branch
# Source: /docs folder

# Manual deployment check
# 1. Verify docs/index.html exists
# 2. Verify docs/.nojekyll exists
# 3. Verify all internal links use relative paths
# 4. Push to main branch
# 5. Check Actions tab for deployment status
```

### Devcontainer
```bash
# Start devcontainer in VS Code
# Press F1 → "Dev Containers: Reopen in Container"

# Or use GitHub Codespaces
# Create codespace from main branch
```

## Testing

### Markdown Link Validation
```bash
# Check for broken internal links
find docs/ -name "*.md" -o -name "*.html" | xargs grep -n "^\[" | grep -v "http"
```

### JSON Validation
```bash
# Validate JSON files
python3 -c "import json; json.load(open('path/to/file.json'))"
```

### YAML Validation
```bash
# Validate YAML files
python3 -c "import yaml; yaml.safe_load(open('path/to/file.yml'))"
```

## Version Control

### Commit Convention
```bash
# Feature
git commit -m "feat: add new feature"

# Fix
git commit -m "fix: correct broken link"

# Documentation
git commit -m "docs: update documentation"

# Chore
git commit -m "chore: update configuration"
```

### Push to Remote
```bash
git push origin main
```

## Common Development Paths

### Documentation Editing
- Root docs: `docs/` directory
- Node.js learning: `aws-cloud-engineer/node-js/` directory

### Agent Configuration
- Skills: `.kilo/skills/`
- Memory: `.kilo/memory/`
- Tasks: `.kilo/tasks/`

### Devcontainer Configuration
- Config: `.devcontainer/devcontainer.json`

### GitHub Actions
- Workflows: `.github/workflows/`

## Tools Installed in Devcontainer

### Runtime
- Node.js LTS
- Python 3
- Java (JDK)
- AWS CLI v2

### Development Tools
- npm (Node Package Manager)
- pip (Python Package Installer)
- git
- GitHub CLI

### AI Agents
- Kilo Code VS Code extension
- Kilo CLI (@kilocode/cli)

## Environment Variables
- `KILO_MODE=code`          # Default agent mode
- `KILO_TELEMETRY=false`    # Disable telemetry (optional)
