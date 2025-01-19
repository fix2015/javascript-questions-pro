## [What is inline caching?](#what-is-inline-caching)

### What is inline caching?

Inline caching is a JavaScript engine optimization technique that speeds up property access by caching the results of previous lookups.

#### Key Points:
1. **Purpose:**
   - Reduce the overhead of repeatedly resolving the same property or method on an object.

2. **How It Works:**
   - During the first lookup, the engine determines the property location and caches it.
   - On subsequent accesses, the engine uses the cached result, bypassing the need for lookup.

Example:
```javascript
function add(a, b) {
  return a.value + b.value;
}

const obj1 = { value: 10 };
const obj2 = { value: 20 };

console.log(add(obj1, obj2)); // Inline caching optimizes property access.
```

**Tags**: advanced, JavaScript, V8 Engine


