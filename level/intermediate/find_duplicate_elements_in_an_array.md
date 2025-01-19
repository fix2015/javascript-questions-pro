## [Find Duplicate Elements in an Array](#find-duplicate-elements-in-an-array)

### Find Duplicate Elements in an Array

To find duplicate elements in an array, use a set to track the elements you've seen as you iterate through the array.

#### Algorithm:
1. Initialize an empty set to store unique elements.
2. Iterate through the array and check if each element is already in the set.
3. If it is, add it to the result array.
4. Return the array of duplicates.

#### Example:
```javascript
function findDuplicates(arr) {
    const seen = new Set();
    const duplicates = [];

    for (const num of arr) {
        if (seen.has(num)) {
            duplicates.push(num);
        }
        seen.add(num);
    }

    return duplicates;
}

// Example usage
console.log(findDuplicates([1, 2, 3, 2, 4, 5, 1])); // Output: [2, 1]
console.log(findDuplicates(["apple", "banana", "apple", "orange"])); // Output: ["apple"]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


