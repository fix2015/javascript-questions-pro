## [Remove Duplicates from an Array](#remove-duplicates-from-an-array)

### Remove Duplicates from an Array

To remove duplicates from an array, you can use a Set, which automatically stores unique values.

#### Algorithm:
1. Convert the array into a Set, which will automatically remove any duplicate values.
2. Convert the Set back into an array.
3. Return the new array with unique elements.

#### Example:
```javascript
function removeDuplicates(arr) {
    return [...new Set(arr)];
}

// Example usage
console.log(removeDuplicates([1, 2, 2, 3, 4, 4, 5])); // Output: [1, 2, 3, 4, 5]
console.log(removeDuplicates(["apple", "banana", "apple", "orange"])); // Output: ["apple", "banana", "orange"]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


