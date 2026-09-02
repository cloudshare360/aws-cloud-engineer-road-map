# Corrections & Decisions

## Package Name Correction
- **Issue**: Initial devcontainer.json used `@kilo-ai/cli` which is incorrect
- **Correct**: Use `@kilocode/cli` (npm package name for Kilo CLI)
- **Verification**: `kilo --version` returns `7.5.6` after install

## GitHub Pages Configuration
- **Issue**: Case-sensitive conflict with both `README.md` and `readme.md` in docs/
- **Fix**: Removed `docs/readme.md`, kept `docs/README.md`, added `docs/index.html`
- **Issue**: GitHub Pages 404 errors
- **Fix**: Created `docs/index.html` as landing page, added `docs/.nojekyll`

## File Structure Changes
- **Decision**: All detailed docs in `docs/` folder, root `readme.md` as index
- **Decision**: Use `NN-` prefix for numbered docs (01-07) for consistent ordering
- **Decision**: `docs/index.html` as GitHub Pages entry point

## Repository Structure
- **Decision**: Create `aws-cloud-engineer/node-js/` for Node.js learning path
- **Decision**: Create `aws-developer/`, `aws-serverless/`, `aws-cloud-engineer/` role folders
- **Decision**: Create `aws-cloud-engineer/aws-services/` with 79 AWS service subdirectories
- **Decision**: Move `aws-developer/` and `aws-serverless/` under `aws-cloud-engineer/` (role combination)
- **Decision**: Remove duplicate root-level `angular/`, `node-js/`, `react/` directories
- **Decision**: Create `node-js/`, `angular/`, `react/` as general folders

## Kilo AI Configuration
- **Decision**: Enable Kilo AI extension and CLI in devcontainer
- **Decision**: Configuration via `devcontainer.json` VS Code settings
- **Decision**: `.kilo/kilo.json` for project-level Kilo configuration
- **Note**: `kilo.json` uses non-standard format; VS Code settings in devcontainer.json are the primary config

## Timeline Correction
- **Decision**: Split Phase 2 into Testing (Weeks 5-6) and Marketing (Weeks 5-8 ongoing)
- **Reason**: Fix overlap between Testing (Weeks 5-8) and Frontend (Weeks 7-8)
