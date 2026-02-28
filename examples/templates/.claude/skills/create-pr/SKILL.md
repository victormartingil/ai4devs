---
name: create-pr
description: Creates a pull request with conventional format
context: fork
agent: code-reviewer
---

# Create Pull Request

## Steps
1. Run `git diff main...HEAD` to understand all changes
2. Analyze the changes and categorize them (feature, fix, refactor, etc.)
3. Generate a PR title following conventional commits format
4. Generate a PR body with:
   - Summary of changes (bullet points)
   - Testing done
   - Breaking changes (if any)
5. Create the PR using `gh pr create`

## PR Body Template
```
## Summary
- [Change description]

## Type
- [ ] Feature
- [ ] Bug fix
- [ ] Refactor
- [ ] Documentation

## Testing
- [How it was tested]

## Breaking Changes
- None
```
