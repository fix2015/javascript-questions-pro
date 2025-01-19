## [What are the optimization techniques of V8 engine?](#what-are-the-optimization-techniques-of-v8-engine)

### What are the optimization techniques of V8 engine?

1. **Just-In-Time (JIT) Compilation:**
   - Converts JavaScript into machine code during runtime.

2. **Hidden Classes:**
   - Creates optimized data structures for objects with the same properties.

3. **Inline Caching:**
   - Speeds up property access by reusing previous lookups.

4. **Garbage Collection:**
   - Automatically reclaims memory no longer in use.

Example:

```javascript
const obj = { a: 1, b: 2 };
console.log(obj.a); // Inline caching used after first lookup
```

**Tags**: advanced, JavaScript, Engines


