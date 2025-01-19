## [Find the Difference Between Two Arrays](#find-the-difference-between-two-arrays)

### Find the Difference Between Two Arrays

To find the difference between two arrays, use a set to track elements that are in one array but not the other.

#### Algorithm:
1. Convert one array into a set for efficient lookup.
2. Iterate through the second array and add elements that are not in the set to the result array.
3. Return the resulting array of differences.

#### Example:
```javascript
function arrayDifference(arr1, arr2) {
    const set = new Set(arr1);
    return arr2.filter(item => !set.has(item));
}

// Example usage
console.log(arrayDifference([1, 2, 3], [3, 4, 5])); // Output: [4, 5]
console.log(arrayDifference([1, 2, 3, 4], [3, 4, 5])); // Output: [5]
```

This method has a time complexity of O(n + m), where n and m are the lengths of the two arrays.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


