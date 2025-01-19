## [What happens If I pass string type for getPrototype method](#what-happens-if-i-pass-string-type-for-getprototype-method)

### What happens If I pass string type for getPrototype method?

If you pass a string type to the `Object.getPrototypeOf()` method, it will throw a `TypeError` because the argument must be an object. The `getPrototypeOf` method only works on objects, and passing a primitive value like a string is invalid.

Example:

```javascript
const str = 'hello';
console.log(Object.getPrototypeOf(str)); // Works fine
console.log(Object.getPrototypeOf('hello')); // TypeError
```

**Tags**: basic, JavaScript, objects


