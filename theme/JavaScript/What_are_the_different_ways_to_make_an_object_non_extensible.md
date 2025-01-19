## [What are the different ways to make an object non-extensible](#what-are-the-different-ways-to-make-an-object-non-extensible)

### What are the different ways to make an object non-extensible?

You can make an object non-extensible in JavaScript in several ways:
- Using `Object.preventExtensions()` makes an object non-extensible.
- Using `Object.seal()` not only prevents extensions but also makes all existing properties non-configurable.
- Using `Object.freeze()` prevents extensions and makes all properties immutable.

Example:

```javascript
const obj = { name: 'John' };
Object.preventExtensions(obj);
console.log(Object.isExtensible(obj)); // false
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


