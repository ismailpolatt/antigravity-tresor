---
description: Technical debt analysis and code health report
---

# /debt-analysis [--scope <path>] [--priority high|medium|low]

## Usage Examples

```bash
/debt-analysis                    # Full project analysis
/debt-analysis --scope src/       # Analyze specific directory
/debt-analysis --priority high    # Focus on critical debt
```

## Analysis Categories

### Code Complexity
- Cyclomatic complexity
- Function length
- Nesting depth
- Class coupling

### Maintainability
- Code duplication
- Dead code
- Outdated patterns
- Missing documentation

### Dependencies
- Outdated packages
- Deprecated APIs
- Security vulnerabilities
- License issues

### Test Coverage
- Coverage gaps
- Untested code paths
- Missing edge cases
- Flaky tests

## Output

### Debt Summary
```
📊 Technical Debt Score: 72/100 (Good)

High Priority: 3 issues
Medium Priority: 8 issues
Low Priority: 15 issues
```

### High Priority Issues
```
🔴 Complex function exceeds threshold
   File: src/utils/parser.ts:145
   Complexity: 25 (threshold: 15)
   Effort: 2 hours

🔴 Duplicated code block
   Files: src/api/users.ts, src/api/posts.ts
   Lines: 45 duplicated lines
   Effort: 1 hour
```

### Recommendations
1. Refactor complex functions
2. Extract shared utilities
3. Update deprecated dependencies
4. Improve test coverage
