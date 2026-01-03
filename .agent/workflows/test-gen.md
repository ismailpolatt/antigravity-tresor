---
description: Generate comprehensive test suites with high coverage targets
---

# /test-gen [--file <path>] [--coverage <percent>] [--type unit|integration|e2e]

## Usage Examples

```bash
/test-gen --file src/utils.ts        # Generate tests for specific file
/test-gen --coverage 90              # Target 90% coverage
/test-gen --type integration         # Focus on integration tests
```

## Test Generation Process

1. **Analysis**
   - Parse source file structure
   - Identify functions, classes, and methods
   - Map code paths and edge cases

2. **Strategy**
   - Determine test framework (Jest, Vitest, pytest, Go test)
   - Plan unit, integration, and E2E tests
   - Identify mock requirements

3. **Generation**
   - Create test files with proper structure
   - Write meaningful test cases
   - Include edge cases and error scenarios
   - Add setup/teardown helpers

## Test Types

### Unit Tests
- Individual function behavior
- Edge cases and error handling
- Mock external dependencies

### Integration Tests
- API endpoint testing
- Database operations
- Service interactions

### E2E Tests
- User flow testing
- Browser/UI testing
- Full system validation

## Output Structure

```
tests/
├── unit/
│   └── utils.test.ts
├── integration/
│   └── api.test.ts
└── e2e/
    └── user-flow.test.ts
```

## Test Templates

### JavaScript/TypeScript (Jest/Vitest)
```typescript
describe('functionName', () => {
  it('should handle normal input', () => {
    expect(functionName('input')).toBe('expected');
  });

  it('should handle edge case', () => {
    expect(() => functionName(null)).toThrow();
  });
});
```

### Python (pytest)
```python
def test_function_name_normal():
    assert function_name('input') == 'expected'

def test_function_name_edge_case():
    with pytest.raises(ValueError):
        function_name(None)
```

## Coverage Targets

| Level | Coverage | Description |
|-------|----------|-------------|
| Minimum | 60% | Basic coverage |
| Standard | 80% | Recommended for production |
| Enterprise | 90%+ | Critical systems |
