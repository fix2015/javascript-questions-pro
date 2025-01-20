## [What are the applications of seal method](#what-are-the-applications-of-seal-method)

### What are the applications of seal method?

`Object.seal()` is commonly used to lock an object to prevent new properties from being added, while still allowing modifications to existing properties. It can be useful in situations where you want to ensure the structure of an object remains unchanged.

Example:

```javascript
const person = { name: 'John' };
Object.seal(person);
person.name = 'Jane'; // Allowed
person.city = 'New York'; // Not allowed
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


