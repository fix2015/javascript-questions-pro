## [How do you prevent an object to extend](#how-do-you-prevent-an-object-to-extend)

### How do you prevent an object to extend?

You can prevent an object from being extended (i.e., from adding new properties) using the `Object.preventExtensions()` method. This method makes the object non-extensible.

Example:

```javascript
const obj = { name: 'John' };
Object.preventExtensions(obj);
obj.age = 30; // Won't be added
console.log(obj); // { name: 'John' }
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


