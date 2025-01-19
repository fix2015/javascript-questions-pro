## [Find the Duplicate Number in an Array](#find-the-duplicate-number-in-an-array)

### Find the Duplicate Number in an Array

To find the duplicate number in an array, use a set to track numbers that have been encountered. If a number is encountered more than once, it's the duplicate.

#### Algorithm:
1. Initialize an empty set to track numbers.
2. Iterate through the array, and for each element, check if it already exists in the set.
3. If it does, return that element as the duplicate.
4. If it does not, add the element to the set.

#### Example:
```javascript
function findDuplicate(arr) {
    const seen = new Set();
    for (let num of arr) {
        if (seen.has(num)) {
            return num;
        }
        seen.add(num);
    }
    return null; // No duplicates found
}

// Example usage
console.log(findDuplicate([1, 2, 3, 4, 5, 3])); // Output: 3
console.log(findDuplicate([1, 2, 3, 4, 5])); // Output: null
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


