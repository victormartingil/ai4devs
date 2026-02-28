---
name: create-pr
description: Creates a PR with Maven build verification
context: fork
agent: code-reviewer
---

# Create Pull Request

## Steps
1. Run `mvn verify` to ensure all tests pass
2. Run `git diff main...HEAD` to understand all changes
3. Analyze changes and categorize (feature, fix, refactor)
4. Generate PR title following conventional commits
5. Generate PR body with summary, testing, breaking changes
6. Create the PR using `gh pr create`

## Pre-checks
- All tests must pass (`mvn verify`)
- No checkstyle violations
- No new TODOs without linked issues

## PR Title Format
`type(scope): description`

Examples:
- `feat(order): add cancel order use case`
- `fix(article): prevent negative stock on update`
- `refactor(infrastructure): extract Kafka adapter`
