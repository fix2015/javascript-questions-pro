## [What is the purpose of seal method](#what-is-the-purpose-of-seal-method)

### What is the purpose of seal method?

The `Object.seal()` method seals an object, preventing new properties from being added, but allowing modification of existing properties. The object is still mutable.

Example:

```javascript
const person = { name: 'John' };
Object.seal(person);
person.name = 'Jane';
console.log(person.name); // 'Jane'
person.age = 30; // This won't work
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458057057950895392](https://www.tiktok.com/@jsmentoring/photo/7458057057950895392)
