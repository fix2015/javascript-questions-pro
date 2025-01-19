## [List down the collection of methods available on WeakSet](#list-down-the-collection-of-methods-available-on-weakset)

### List down the collection of methods available on WeakSet

The `WeakSet` object supports the following methods:

- `add(value)` – Adds a value to the set.
- `delete(value)` – Removes a value from the set.
- `has(value)` – Checks if a value is in the set.

Example:

```javascript
const obj = { name: 'John' };
const weakset = new WeakSet([obj]);
weakset.add(obj);
console.log(weakset.has(obj)); // true
weakset.delete(obj);
console.log(weakset.has(obj)); // false
```

**Tags**: basic, JavaScript, collections

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458291433980579105](https://www.tiktok.com/@jsmentoring/photo/7458291433980579105)
