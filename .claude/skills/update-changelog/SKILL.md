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
1. Run `git diff --staged` to understand what is changing
2. If `CHANGELOG.md` does not exist, create it with the structure below
3. Add a concise entry under the appropriate type inside `[Unreleased]`
4. Stage the file: `git add CHANGELOG.md`

## Format
```markdown
# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added
- Example new feature

## [1.0.0] - YYYY-MM-DD

### Added
- Initial release
```
