## [What is a spread operator](#what-is-a-spread-operator)

### What is a spread operator?

The spread operator (`...`) is used to expand elements of an array or object. It can be used to create shallow copies or merge multiple arrays or objects.

Example with arrays:

```javascript
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5];
console.log(arr2); // [1, 2, 3, 4, 5]
```
Example with objects:

```javascript
const obj1 = { name: 'John', age: 30 };
const obj2 = { ...obj1, city: 'New York' };
console.log(obj2); // { name: 'John', age: 30, city: 'New York' }
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [operators](./theme/operators)


