---
name: review
description: Review code for TypeScript/React standards compliance
---

Use @react-code-std to review code and report:

1. **Violations by category:**

   - Types (interface vs type, import type, naming)
   - Naming (PascalCase, camelCase, prefixes)
   - Components (displayName, memoization, patterns)
   - Hooks (export style, return format, dependencies)
   - Style (any usage, const/let, TypeScript strict)

2. **Severity levels:**

   - Critical: Type safety issues, breaking patterns
   - Medium: Missing optimizations, naming inconsistencies
   - Low: Style preferences, minor improvements

3. **Line-by-line issues with suggested fixes**

4. **Compliance rating (0-100%)**

Format output as:

```
## Review Results

**Compliance:** XX%

### Critical Issues
- [Line X] Description → Suggested fix

### Medium Issues
...

### Low Issues
...
```
