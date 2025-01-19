## [What is optional chaining?](#what-is-optional-chaining)

### What is optional chaining?

The optional chaining operator (`?.`) allows safe access to deeply nested object properties without worrying about `null` or `undefined` errors.

Example:

```javascript
const user = { profile: { name: 'Alice' } };
console.log(user.profile?.name); // 'Alice'
console.log(user.address?.street); // undefined
```

**Tags**: basic, JavaScript, Operators


