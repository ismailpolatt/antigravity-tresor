---
description: Generate conventional commit messages for staged changes
---

# /commit [--type feat|fix|docs|refactor|test]

## Usage Examples

```bash
/commit                    # Auto-detect commit type
/commit --type feat        # Force feature commit
/commit --type fix         # Force fix commit
```

## Process

1. **Analyze Changes**
   - Run `git diff --staged`
   - Identify changed files
   - Understand scope of changes

2. **Determine Type**
   - feat: New feature
   - fix: Bug fix
   - docs: Documentation
   - refactor: Code restructure
   - test: Test changes
   - chore: Maintenance

3. **Generate Message**
   - Create subject line (50 chars max)
   - Add body if needed
   - Include breaking change note if applicable

## Commit Types

| Type | Description | Example |
|------|-------------|---------|
| `feat` | New feature | feat(auth): add OAuth login |
| `fix` | Bug fix | fix(api): handle null response |
| `docs` | Documentation | docs: update API guide |
| `refactor` | Restructure | refactor(utils): simplify parser |
| `test` | Tests | test(auth): add login tests |
| `chore` | Maintenance | chore: update dependencies |

## Format

```
<type>(<scope>): <subject>

[optional body]

[optional footer]
```

## Examples

```bash
# Feature
feat(user): add profile picture upload

# Fix
fix(api): resolve timeout on large requests

Increased timeout from 30s to 60s for file uploads.
Closes #123

# Breaking Change
feat(auth)!: migrate to OAuth 2.0

BREAKING CHANGE: JWT tokens are no longer supported.
```
