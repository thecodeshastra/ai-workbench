# AI-Workbench Change logs

---

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-02-18

### Tombstoned [Depricated]

---

## [0.1.0] - 2026-02-18

### Changed

- Migrated dependency management from `requirements.txt` to `pyproject.toml` using `uv`.
- Updated `README.md` with `uv` installation and usage commands.
- Updated `.gitignore` to exclude MkDocs build output (`site/`).

### Added

- Added `[project.scripts]` entry points for `stateless-agent`, `summarizer-agent`, `virtual-assistant`, and `virtual-assistant-chatbot`.
- Added GitHub Actions workflow (`.github/workflows/deploy-docs.yml`) for automatic MkDocs deployment.
- Added optional test dependencies (`pytest`, `pytest-cov`).
