## [What are the differences between freeze and seal methods](#what-are-the-differences-between-freeze-and-seal-methods)

### What are the differences between freeze and seal methods?

Both `Object.freeze()` and `Object.seal()` prevent modification of an object, but with different restrictions:

- `Object.freeze()` makes an object immutable, preventing changes to existing properties, and disallowing the addition or removal of properties.
- `Object.seal()` allows modification of existing properties but prevents the addition of new properties.

Example:

```javascript
const obj1 = { name: 'John' };
Object.freeze(obj1);
obj1.name = 'Jane'; // Not allowed
obj1.age = 30; // Not allowed

const obj2 = { name: 'John' };
Object.seal(obj2);
obj2.name = 'Jane'; // Allowed
obj2.age = 30; // Not allowed
```

**Tags**: basic, JavaScript, objects


