---
description: Comprehensive code review for staged changes with security and performance checks
---

# /review [--scope staged|all|file] [--checks security,performance,quality]

## Usage Examples

```bash
/review                          # Review staged changes
/review --scope all              # Review all modified files
/review --checks security        # Focus on security issues only
/review --scope file src/api.ts  # Review specific file
```

## Review Process

1. **Context Gathering**
   - Run `git diff --staged` for staged changes
   - Run `git status` to understand current state
   - Identify modified files and their types

2. **Analysis Categories**

### Security (Critical)
- SQL injection, XSS, CSRF vulnerabilities
- Hardcoded secrets or API keys
- Input validation issues
- Authentication/authorization flaws

### Performance (High)
- N+1 query problems
- Memory leaks
- Inefficient algorithms
- Missing caching opportunities

### Code Quality (High)
- Readability and maintainability
- Proper error handling
- Consistent patterns and style
- Documentation completeness

### Testing
- Test coverage for new code
- Edge case handling
- Meaningful assertions

## Output Format

### Executive Summary
- Overall assessment
- Critical issues count
- Key recommendations

### Critical Issues (Must Fix)
```
🔴 [SECURITY] SQL Injection in user input
   File: src/db/queries.ts:45
   Fix: Use parameterized queries
```

### Important Issues (Should Fix)
```
🟡 [PERFORMANCE] N+1 query in posts loop
   File: src/api/posts.ts:23
   Fix: Use batch loading with includes
```

### Suggestions (Consider)
```
🔵 [QUALITY] Complex function, consider refactoring
   File: src/utils/parser.ts:78
```

### Action Plan
1. **Immediate**: Security and critical bugs
2. **Before Merge**: Performance and quality issues
3. **Future**: Refactoring and optimization suggestions
