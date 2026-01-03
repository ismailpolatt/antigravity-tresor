---
description: Performance profiling and optimization analysis
---

# /profile [--type cpu|memory|network] [--file <path>]

## Usage Examples

```bash
/profile                        # Full performance analysis
/profile --type memory          # Focus on memory usage
/profile --file src/api.ts      # Profile specific file
```

## Analysis Types

### CPU Profiling
- Hot paths identification
- Loop optimization opportunities
- Algorithm efficiency analysis
- Async/await bottlenecks

### Memory Analysis
- Memory leak detection
- Unnecessary allocations
- Object lifecycle issues
- Garbage collection pressure

### Network Analysis
- API call optimization
- Request batching opportunities
- Caching recommendations
- Payload size analysis

## Process

1. **Static Analysis**
   - Identify expensive operations
   - Check algorithm complexity
   - Review data structures

2. **Pattern Detection**
   - N+1 query problems
   - Unnecessary re-renders (React)
   - Blocking operations
   - Memory leaks

3. **Recommendations**
   - Optimization suggestions
   - Caching strategies
   - Code refactoring tips

## Output

### Performance Issues
```
🔴 HIGH: N+1 query in loop
   File: src/api/posts.ts:23
   Impact: 100ms+ per additional item
   Fix: Use batch loading
```

### Optimization Opportunities
```
🟡 MEDIUM: Heavy computation in render
   File: src/components/List.tsx:45
   Fix: Memoize with useMemo
```

### Best Practices
```
🔵 TIP: Consider lazy loading
   File: src/pages/Dashboard.tsx
   Benefit: Reduced initial bundle
```
