---
name: complexity-analyzer
description: Measure cyclomatic complexity, cognitive complexity, and coupling metrics. Identify the highest-risk files for refactoring.
---

# Complexity Analyzer

## When to use

- Before planning a refactoring sprint
- When estimating effort for changes in a module
- During code review of complex logic
- For prioritizing technical debt paydown

## Metrics to measure

1. **Cyclomatic Complexity** - Number of linearly independent paths (target: < 10)
2. **Cognitive Complexity** - How hard code is to understand (target: < 15)
3. **Lines of Code** per function and file
4. **Depth of Inheritance** - Class hierarchy depth (target: < 4)
5. **Coupling Between Objects** - Number of classes a class depends on
6. **Lack of Cohesion** - Methods in a class that don't share data
7. **Halstead Metrics** - Volume, difficulty, effort estimates

## Instructions

1. Run complexity analysis across all source files
2. Rank files by complexity score
3. Identify hotspots - high complexity + high change frequency
4. Estimate refactor effort per file
5. Suggest specific refactoring techniques:
   - Extract Method for long functions
   - Replace Conditional with Polymorphism for complex switches
   - Introduce Parameter Object for long parameter lists

## Output

- Complexity leaderboard (top 20 most complex files)
- Hotspot map (complexity × churn rate)
- Estimated total refactor effort in days
- Prioritized refactoring backlog
