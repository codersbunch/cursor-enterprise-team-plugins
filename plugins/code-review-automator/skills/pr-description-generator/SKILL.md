---
name: pr-description-generator
description: Generate comprehensive pull request descriptions from git diff, commit messages, and ticket context.
---

# PR Description Generator

## When to use

- Before opening a pull request
- When updating a draft PR description
- For standardizing PR descriptions across the team

## Instructions

1. **Analyze the diff** - understand what changed and why
2. **Read commit messages** for context on intent
3. **Generate description** with:
   - **Summary**: One-line description of the change
   - **Motivation**: Why this change was needed
   - **Changes**: Bullet list of what was modified
   - **Testing**: How to verify the change works
   - **Screenshots**: Placeholder if UI was changed
   - **Checklist**: Standard review checklist
4. **Link ticket** - extract ticket number from branch name
5. **Suggest labels** - bug, feature, refactor, docs, etc.
6. **Estimate review effort** - Small/Medium/Large based on diff size

## Output format

```markdown
## Summary
Brief description of what this PR does.

## Motivation
Why this change is needed.

## Changes
- Added X to support Y
- Refactored Z for better readability

## Testing
1. Step to test
2. Expected result

Closes #123
```
