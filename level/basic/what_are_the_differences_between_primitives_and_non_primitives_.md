## [What are the differences between primitives and non-primitives?](#what-are-the-differences-between-primitives-and-non-primitives)

### What are the differences between primitives and non-primitives?

**Primitives**:
- Immutable, basic data types (e.g., `string`, `number`, `boolean`, `null`, `undefined`, `Symbol`, `BigInt`).
- Stored directly in memory.

**Non-primitives**:
- Objects, arrays, and functions.
- Mutable and stored as references in memory.

Example:

```javascript
let a = 10; // Primitive
let b = a;
b = 20;
console.log(a); // 10 (no change)

let obj = { key: 'value' }; // Non-primitive
let ref = obj;
ref.key = 'newValue';
console.log(obj.key); // 'newValue' (reference changed)
```

**Tags**: basic, JavaScript, Data Types


