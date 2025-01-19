## [How do you list all properties of an object](#how-do-you-list-all-properties-of-an-object)

### How do you list all properties of an object?

You can list all properties of an object in JavaScript using methods like `Object.keys()`, `Object.getOwnPropertyNames()`, or `for...in` loops.

Example using `Object.keys()`:

```javascript
const person = { name: 'John', age: 30 };
console.log(Object.keys(person)); // ['name', 'age']
```
Example using `for...in` loop:

```javascript
const person = { name: 'John', age: 30 };
for (let key in person) {
  console.log(key); // name, age
}
```

**Tags**: intermediate, JavaScript, objects


