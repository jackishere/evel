---
name: update-changelog
description: Update CHANGELOG.md following the Keep a Changelog 1.1.0 specification before committing
---

Update `CHANGELOG.md` to reflect the current changes, following [Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/).

## Rules
- File is named `CHANGELOG.md` at the project root
- Latest version at the top; `[Unreleased]` section always first
- Dates in ISO 8601 format: `YYYY-MM-DD`
- Group entries under the correct type — only include types that have entries:
  - `Added` — new features
  - `Changed` — changes to existing functionality
  - `Deprecated` — soon-to-be removed features
  - `Removed` — removed features
  - `Fixed` — bug fixes
  - `Security` — vulnerability fixes

## Steps
1. Run `git diff` and `git status` to understand what is changing
2. Read `package.json` to get the `name` and `version` fields
3. Get today's date in ISO 8601 format (`YYYY-MM-DD`)
4. If `CHANGELOG.md` does not exist, create it with the structure below
5. **Physically write the new entry into `CHANGELOG.md`** using the Edit or Write tool — do not just describe what should be added
6. **Always** print the new lines added to `CHANGELOG.md` to the developer — mandatory, never skip

## Entry prefix format
Each entry must be prefixed with service name, version, and date:
```
- [evel v1.0.0 - 2024-01-15] Description of the change
```

## Format
```markdown
# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added
- [evel v1.0.0 - YYYY-MM-DD] Example new feature

## [1.0.0] - YYYY-MM-DD

### Added
- [evel v1.0.0 - YYYY-MM-DD] Initial release
```
