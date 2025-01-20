## [How do you define multiple properties on an object](#how-do-you-define-multiple-properties-on-an-object)

### How do you define multiple properties on an object?

You can define multiple properties on an object in JavaScript by using either object literal syntax or `Object.defineProperties()` method.

Example using object literal:

```javascript
const person = { name: 'John', age: 30 };
```

Example using `Object.defineProperties()`:

```javascript
const person = {};
Object.defineProperties(person, {
  name: { value: 'John', writable: true },
  age: { value: 30, writable: true }
});
console.log(person);
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


