---
name: create-draft-pr
description: Create a draft pull request with AI-generated description, suggested reviewers, and labels.
---

# Create Draft PR

Automatically create a draft PR with complete metadata.

## Steps

1. Check current branch has commits ahead of base branch
2. Generate PR description from diff and commit messages
3. Suggest reviewers from CODEOWNERS and git history
4. Detect appropriate labels from changed files
5. Create draft PR via GitHub CLI:
   `gh pr create --draft --title "..." --body "..." --reviewer "..."`
6. Post link to PR in terminal
