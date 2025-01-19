## [What is the purpose of compareFunction while sorting arrays](#what-is-the-purpose-of-comparefunction-while-sorting-arrays)

### What is the purpose of compareFunction while sorting arrays?

The `compareFunction` in the `sort()` method allows you to define custom sorting logic. By default, `sort()` converts elements to strings and sorts them lexicographically. The `compareFunction` allows you to specify how the elements should be compared, typically using numerical comparison.

Example:

```javascript
const arr = [3, 1, 2];
arr.sort((a, b) => a - b);
console.log(arr); // [1, 2, 3]
```

**Tags**: basic, JavaScript, arrays


