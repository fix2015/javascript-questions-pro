## [Find the First Index of an Element in an Array](#find-the-first-index-of-an-element-in-an-array)

### Find the First Index of an Element in an Array

To find the first index of an element in an array, you can use the `indexOf` method.

#### Algorithm:
1. Use the `indexOf` method to search for the element in the array.
2. If the element is found, return its index.
3. If the element is not found, return `-1`.

#### Example:
```javascript
function findFirstIndex(arr, elem) {
    return arr.indexOf(elem);
}

// Example usage
console.log(findFirstIndex([1, 2, 3, 4], 3)); // Output: 2
console.log(findFirstIndex(["apple", "banana", "cherry"], "banana")); // Output: 1
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


