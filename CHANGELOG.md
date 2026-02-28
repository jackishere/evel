# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Changed
- [evel v1.0.0 - 2026-02-28] code-commiter agent switched to haiku model

### Fixed
- [evel v1.0.0 - 2026-02-28] code-commiter agent and update-changelog skill now correctly write CHANGELOG.md and include it in every commit

### Added
- `code-commiter` agent with conventional commits and changelog update skills
- `update-changelog` skill following Keep a Changelog 1.1.0
- `conventional-commit` skill for standardized commit messages
- Distroless multi-stage Dockerfile
- `.dockerignore` excluding node_modules, .git, .claude
- `CLAUDE.md` with project rules and commit conventions

### Changed
- `code-commiter` agent now presents changelog diff to developer before outputting commit commands
- `code-commiter` agent only invoked on explicit developer request
