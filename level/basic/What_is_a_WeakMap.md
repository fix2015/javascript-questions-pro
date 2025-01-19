## [What is a WeakMap](#what-is-a-weakmap)

### What is a WeakMap?

A `WeakMap` is a collection of key-value pairs where the keys are objects and the values can be any type. The keys in a `WeakMap` are held weakly, meaning they can be garbage collected when there are no other references to the key object.

Example:

```javascript
const obj1 = { name: 'John' };
const weakmap = new WeakMap();
weakmap.set(obj1, 'value');
console.log(weakmap.get(obj1)); // 'value'
```

**Tags**: basic, JavaScript, collections

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458221758114516256](https://www.tiktok.com/@jsmentoring/photo/7458221758114516256)
