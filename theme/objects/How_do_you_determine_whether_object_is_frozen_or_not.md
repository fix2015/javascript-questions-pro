## [How do you determine whether object is frozen or not](#how-do-you-determine-whether-object-is-frozen-or-not)

### How do you determine whether object is frozen or not?

You can use `Object.isFrozen()` to check if an object is frozen. A frozen object cannot have its properties modified, added, or removed.

Example:

```javascript
const person = { name: 'John' };
Object.freeze(person);
console.log(Object.isFrozen(person)); // true
```

**Tags**: basic, JavaScript, objects

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457681827478785312](https://www.tiktok.com/@jsmentoring/photo/7457681827478785312)
