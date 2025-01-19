## [What are the differences between WeakSet and Set](#what-are-the-differences-between-weakset-and-set)

### What are the differences between WeakSet and Set?

- A `WeakSet` holds weak references to its objects, which allows garbage collection when the objects are no longer referenced elsewhere.
- A `Set` holds strong references to its elements, preventing garbage collection until the set itself is garbage collected.
- `WeakSet` can only store objects, while `Set` can store any type of value.

Example:

```javascript
const obj1 = { name: 'John' };
const weakset = new WeakSet([obj1]);
const set = new Set([obj1]);
```

**Tags**: basic, JavaScript, collections

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458240152905846048](https://www.tiktok.com/@jsmentoring/photo/7458240152905846048)
