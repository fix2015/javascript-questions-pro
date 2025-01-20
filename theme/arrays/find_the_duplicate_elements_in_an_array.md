## [Find the Duplicate Elements in an Array](#find-the-duplicate-elements-in-an-array)

### Find the Duplicate Elements in an Array

To find duplicate elements in an array, you can use a frequency map or set to track the elements that have already been encountered.

#### Algorithm:
1. Create a set to store elements you've seen.
2. Iterate through the array and check if an element is already in the set.
3. If it is, add it to the result array.
4. If not, add it to the set.
5. Return the result array with duplicates.

#### Example:
```javascript
function findDuplicates(arr) {
    let seen = new Set(), duplicates = [];
    for (let num of arr) {
        if (seen.has(num)) {
            duplicates.push(num);
        } else {
            seen.add(num);
        }
    }
    return duplicates;
}

// Example usage
console.log(findDuplicates([1, 2, 3, 1, 4, 5, 3])); // Output: [1, 3]
console.log(findDuplicates([10, 20, 30, 40])); // Output: []
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


