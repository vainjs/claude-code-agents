---
name: generate
description: Generate TypeScript/React code following standards
---

Use @react-code-std to generate compliant code:

**Process:**

1. Clarify requirements and component/hook purpose
2. Apply all standards from @react-code-std strictly
3. Add minimal comments (only for complex logic)
4. Provide usage example

**Ensure:**

- Use `type` not `interface`
- Import types with `import type`
- Proper naming: `ComponentNameProps`, `useHookName`
- Set `displayName` for components
- Memoize callbacks and expensive computations
- Organize imports: types → libraries → components → utilities
- TypeScript strict mode compliance

**Output format:**

```typescript
// Generated code here
```

**Usage example:**

```typescript
// How to use the generated code
```

**Standards applied:** [List key standards used]
