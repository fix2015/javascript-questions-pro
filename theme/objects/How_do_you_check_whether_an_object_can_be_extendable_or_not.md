## [How do you check whether an object can be extendable or not](#how-do-you-check-whether-an-object-can-be-extendable-or-not)

### How do you check whether an object can be extendable or not?

You can check whether an object is extensible (i.e., if new properties can be added) using the `Object.isExtensible()` method. This method returns `true` if the object is extensible, and `false` if it is not.

Example:

```javascript
const obj = {};
console.log(Object.isExtensible(obj)); // true
Object.preventExtensions(obj);
console.log(Object.isExtensible(obj)); // false
```

**Tags**: basic, JavaScript, objects


