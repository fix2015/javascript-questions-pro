## [Do all objects have prototypes](#do-all-objects-have-prototypes)

### Do all objects have prototypes?

Yes, in JavaScript, all objects inherit from `Object.prototype` by default, which means they have access to its methods and properties. However, objects created with `Object.create(null)` do not have a prototype.

Example:

```javascript
let obj = {};
console.log(Object.getPrototypeOf(obj));  // Output: [object Object]
```

**Tags**: intermediate, JavaScript, Objects


