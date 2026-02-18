---
name: estimate-refactor-effort
description: Estimate the effort required to refactor a specific module or file based on complexity metrics and code smells.
---

# Estimate Refactor Effort

Analyze a module and produce a detailed effort estimate for refactoring.

## Steps

1. Run complexity metrics on target file/module
2. Count and categorize code smells
3. Identify dependencies that would be affected
4. Estimate test coverage needed after refactor
5. Calculate effort breakdown:
   - Analysis and planning
   - Implementation
   - Testing
   - Code review
6. Identify risks and unknowns
7. Output estimate with confidence level (High/Medium/Low)
