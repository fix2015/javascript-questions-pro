## [What is a WeakSet](#what-is-a-weakset)

### What is a WeakSet?

A `WeakSet` is a collection of objects where each object is held weakly. This means the objects in a `WeakSet` are not prevented from being garbage-collected when there are no other references to them. It only accepts objects, and it does not allow duplicates.

Example:

```javascript
const obj1 = { name: 'John' };
const obj2 = { name: 'Jane' };
const weakset = new WeakSet([obj1, obj2]);
console.log(weakset.has(obj1)); // true
```

**Tags**: basic, JavaScript, collections


