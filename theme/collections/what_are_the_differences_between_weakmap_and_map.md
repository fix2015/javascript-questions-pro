## [What are the differences between WeakMap and Map](#what-are-the-differences-between-weakmap-and-map)

### What are the differences between WeakMap and Map?

- A `WeakMap` holds key-value pairs where the keys are objects and are held weakly, meaning they can be garbage collected if no other references exist.
- A `Map` holds key-value pairs where the keys can be of any data type and are held strongly.

Example:

```javascript
const obj = { name: 'John' };
const weakmap = new WeakMap();
const map = new Map();
weakmap.set(obj, 'value');
map.set(obj, 'value');
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [collections](./theme/collections)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458189087422401825](https://www.tiktok.com/@jsmentoring/photo/7458189087422401825)
