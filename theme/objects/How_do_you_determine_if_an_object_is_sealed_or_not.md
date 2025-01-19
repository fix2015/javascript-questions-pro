## [How do you determine if an object is sealed or not](#how-do-you-determine-if-an-object-is-sealed-or-not)

### How do you determine if an object is sealed or not?

You can use `Object.isSealed()` to check if an object is sealed. A sealed object cannot have new properties added to it, but its existing properties can be modified.

Example:

```javascript
const person = { name: 'John' };
Object.seal(person);
console.log(Object.isSealed(person)); // true
```

**Tags**: basic, JavaScript, objects


