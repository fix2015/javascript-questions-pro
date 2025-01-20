## [How do you sort elements in an array](#how-do-you-sort-elements-in-an-array)

### How do you sort elements in an array?

You can sort elements in an array using the `sort()` method in JavaScript. The `sort()` method sorts the array in place, and you can pass a compare function to customize the sorting order.

Example:

```javascript
const arr = [3, 1, 2];
arr.sort();
console.log(arr); // ['1', '2', '3']

arr.sort((a, b) => a - b);
console.log(arr); // [1, 2, 3]
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [arrays](./theme/arrays)


