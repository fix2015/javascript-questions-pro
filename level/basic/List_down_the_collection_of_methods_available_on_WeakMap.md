## [List down the collection of methods available on WeakMap](#list-down-the-collection-of-methods-available-on-weakmap)

### List down the collection of methods available on WeakMap

The `WeakMap` object supports the following methods:

- `set(key, value)` – Adds a key-value pair.
- `get(key)` – Retrieves the value associated with the key.
- `has(key)` – Checks if a key exists in the `WeakMap`.
- `delete(key)` – Removes a key-value pair.

Example:

```javascript
const obj = { name: 'John' };
const weakmap = new WeakMap();
weakmap.set(obj, 'value');
console.log(weakmap.get(obj)); // 'value'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [collections](./theme/collections)


