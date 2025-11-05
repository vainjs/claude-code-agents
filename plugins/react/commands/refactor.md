---
name: refactor
description: Refactor code to align with TypeScript/React standards
---

Use @react-code-std to refactor code following these steps:

**1. Identify violations with line numbers:**

- Types: interface → type, missing `import type`, naming
- Naming: incorrect PascalCase/camelCase, missing prefixes
- Components: missing displayName, no memoization, wrong export
- Hooks: wrong export style, array returns, missing dependencies
- Style: `any` usage, `let` vs `const`, missing TypeScript strict

**2. Prioritize fixes:**

- Phase 1: Type safety (interface → type, any → specific types)
- Phase 2: Naming conventions (all naming fixes)
- Phase 3: Patterns (memoization, displayName, structure)

**3. Show refactoring plan:**

```
## Refactoring Plan

### Phase 1: Type Safety
- [Line X] Convert interface to type
- [Line Y] Replace any with specific type

### Phase 2: Naming
...

### Phase 3: Patterns
...
```

**4. Apply changes incrementally with before/after:**

```typescript
// Before
interface Props { ... }

// After
type ButtonProps = { ... }
```

**5. Flag breaking changes:**

- Exported interface → type (may affect imports)
- Function signature changes
- Component API changes

**Important:** Ask for confirmation before applying breaking changes.
