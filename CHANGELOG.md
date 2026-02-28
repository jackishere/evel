# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

## [1.0.0] - 2026-02-28

### Added
- [evel v1.0.0 - 2026-02-28] Express server with `/health` and `POST /echo` endpoints
- [evel v1.0.0 - 2026-02-28] `code-commiter` agent with conventional commits and changelog update skills
- [evel v1.0.0 - 2026-02-28] `update-changelog` skill following Keep a Changelog 1.1.0
- [evel v1.0.0 - 2026-02-28] `conventional-commit` skill for standardized commit messages
- [evel v1.0.0 - 2026-02-28] Distroless multi-stage Dockerfile and `.dockerignore`
- [evel v1.0.0 - 2026-02-28] `CLAUDE.md` with project rules and commit conventions

### Changed
- [evel v1.0.0 - 2026-02-28] `code-commiter` agent switched to haiku model
- [evel v1.0.0 - 2026-02-28] `code-commiter` agent only invoked on explicit developer request
- [evel v1.0.0 - 2026-02-28] `code-commiter` agent presents changelog diff before outputting commit commands

### Fixed
- [evel v1.0.0 - 2026-02-28] `code-commiter` agent and `update-changelog` skill now correctly write CHANGELOG.md and include it in every commit
