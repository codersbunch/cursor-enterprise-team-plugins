---
name: reviewer-suggester
description: Suggest the best reviewers for a PR based on code ownership, expertise, and availability using CODEOWNERS and git history.
---

# Reviewer Suggester

## When to use

- Before requesting review on a PR
- When unsure who owns a particular module
- For distributing review load across the team

## Instructions

1. **Analyze changed files** in the PR diff
2. **Check CODEOWNERS** file for explicit ownership
3. **Analyze git blame** - who last modified these files
4. **Check git log** - who has reviewed similar changes before
5. **Consider workload** - avoid reviewers with many open review requests
6. **Suggest 2-3 reviewers** with reasoning:
   - Primary: Code owner or domain expert
   - Secondary: Someone who reviewed similar code recently
   - Optional: Senior reviewer for high-risk changes

## Output

- Ranked list of suggested reviewers
- Reason for each suggestion
- Files each reviewer owns or has expertise in
- Current review load (open PRs awaiting their review)
