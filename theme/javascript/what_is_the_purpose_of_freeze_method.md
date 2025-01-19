## [What is the purpose of freeze method](#what-is-the-purpose-of-freeze-method)

### What is the purpose of freeze method?

The purpose of `Object.freeze()` is to make an object immutable. Once an object is frozen, you cannot alter its properties or add new ones, ensuring the integrity of the data.

Example:

```javascript
const obj = { key: 'value' };
Object.freeze(obj);
obj.key = 'new value'; // Won't work
```

**Tags**: basic, JavaScript, objects


