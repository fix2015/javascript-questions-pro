## [Find Unique Elements in an Array](#find-unique-elements-in-an-array)

### Find Unique Elements in an Array

To find unique elements in an array, you can use a set to filter out duplicates.

#### Algorithm:
1. Convert the array to a set, which automatically removes duplicates.
2. Convert the set back to an array to get the unique elements.
3. Return the unique array.

#### Example:
```javascript
function findUnique(arr) {
    return [...new Set(arr)];
}

// Example usage
console.log(findUnique([1, 2, 2, 3, 4, 4])); // Output: [1, 2, 3, 4]
console.log(findUnique(["apple", "banana", "apple"])); // Output: ["apple", "banana"]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


