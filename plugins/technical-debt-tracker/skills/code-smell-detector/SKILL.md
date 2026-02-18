---
name: code-smell-detector
description: Identify code smells including long methods, duplicate code, large classes, feature envy, and other maintainability issues.
---

# Code Smell Detector

## When to use

- During quarterly tech debt reviews
- Before major refactoring sprints
- When onboarding to a legacy codebase
- When code review velocity slows down

## Code smells to detect

1. **Long Method** - Functions over 50 lines
2. **Large Class** - Classes over 300 lines with too many responsibilities
3. **Duplicate Code** - Similar blocks repeated across files
4. **Long Parameter List** - Functions with more than 4 parameters
5. **Feature Envy** - Method uses another class's data more than its own
6. **Data Clumps** - Same group of variables appearing together repeatedly
7. **Primitive Obsession** - Using primitives instead of small objects
8. **Switch Statements** - Large switch/if-else chains that should be polymorphism
9. **Dead Code** - Unused variables, functions, imports, exports
10. **Speculative Generality** - Over-engineered abstractions not currently needed
11. **TODO/FIXME debt** - Stale comments without associated tickets
12. **Magic Numbers** - Unexplained numeric literals

## Output

- Smell type and location
- Severity: High/Medium/Low
- Estimated refactor effort: Hours
- Suggested refactoring pattern
- Priority score (severity × frequency × business impact)
