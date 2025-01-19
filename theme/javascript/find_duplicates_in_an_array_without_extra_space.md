## [Find Duplicates in an Array Without Extra Space](#find-duplicates-in-an-array-without-extra-space)

### Find Duplicates in an Array Without Extra Space

To find duplicates without using extra space, you can modify the array in-place.

#### Algorithm:
1. Iterate through the array and use the value of each element as an index.
2. If the value at that index is negative, it means the element has been seen before, so it is a duplicate.
3. If the value at that index is positive, make it negative to mark it as visited.
4. Return the duplicates.

#### Example:
```javascript
function findDuplicatesInPlace(arr) {
    const duplicates = [];
    for (let i = 0; i < arr.length; i++) {
        const absVal = Math.abs(arr[i]);
        if (arr[absVal] < 0) {
            duplicates.push(absVal);
        } else {
            arr[absVal] = -arr[absVal];
        }
    }
    return duplicates;
}

// Example usage
console.log(findDuplicatesInPlace([4, 3, 2, 7, 8, 2, 3, 1])); // Output: [2, 3]
console.log(findDuplicatesInPlace([1, 1, 1, 2, 2])); // Output: [1, 2]
```

This method has a time complexity of O(n), where n is the length of the array, and does not use extra space.

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


