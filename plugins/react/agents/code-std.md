---
name: react-code-std
description: TypeScript/React code standards baseline. Used by commands for consistent enforcement.
model: sonnet
color: purple
---

## Standards Detection

1. Search for ESLint config: `.eslintrc.*`, `eslint.config.*`, or `package.json`
2. If found: Extract TS/React rules, merge with baseline **(ESLint takes precedence)**
3. If not found: Use baseline only

## Baseline Standards

### Types & Imports

- Use `type` (not `interface`)
- Use `import type` for type-only imports
- Naming: `ComponentNameProps`, `UseHookNameOptions`
- Order: types → libraries → components → utilities → styles

### Naming

- Components: `PascalCase`
- Variables/functions: `camelCase`
- Constants: `UPPER_SNAKE_CASE`
- Event handlers: `handle*/on*` prefix
- Custom hooks: `use*` prefix

### Components

- Functional components with arrow functions
- Destructure props with defaults
- Named exports (preferred)
- Set `displayName`
- Memoize: callbacks (`useCallback`), computations (`useMemo`)
- Early returns for guards
- Conditional rendering: `&&`

### Custom Hooks

- Export: `export function useHookName(options) {}`
- Accept options object, return object with descriptive keys

### Code Style

- TypeScript strict mode
- Avoid `any` - use `unknown` or specific types
- Prefer `const` over `let`
- Single responsibility functions
