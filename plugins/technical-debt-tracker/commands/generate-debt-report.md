---
name: generate-debt-report
description: Generate a comprehensive technical debt report with complexity metrics, code smells, and a prioritized refactoring backlog.
---

# Generate Debt Report

Analyze the codebase and produce an actionable technical debt report.

## Steps

1. Run complexity analysis across all source files
2. Detect code smells (long methods, duplicates, dead code)
3. Check for stale TODO/FIXME comments
4. Audit outdated dependencies
5. Measure test coverage gaps
6. Calculate debt score per module
7. Rank by priority (complexity x churn rate)
8. Generate prioritized backlog with effort estimates
9. Output report to `tech-debt-report.md`
10. Optionally create Jira/Linear tickets for top 10 items
