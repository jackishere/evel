---
name: conventional-commit
description: Stage changes and commit using the Conventional Commits specification
argument-hint: "[optional message]"
---

Create a git commit following the Conventional Commits specification.

## Format
```
<type>(<scope>): <description>

[optional body]
```

## Types
- `feat` — new feature
- `fix` — bug fix
- `docs` — documentation only
- `refactor` — code change that is not a fix or feature
- `test` — adding or updating tests
- `chore` — build process, tooling, config

## Steps
1. Run `git diff --staged` and `git status` to understand what's changed
2. If nothing is staged, stage relevant files first
3. Choose the appropriate type and optional scope
4. Write a concise description in lowercase, imperative mood
5. Commit with: `git commit -m "<type>(<scope>): <description>"`

If `$ARGUMENTS` is provided, use it as a hint for the description.
