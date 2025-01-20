## [Find the Duplicate Element in an Array](#find-the-duplicate-element-in-an-array)

### Find the Duplicate Element in an Array

To find a duplicate element in an array, use a set to track the elements that have been seen. If an element is already in the set, it's a duplicate.

#### Algorithm:
1. Create an empty set to store elements.
2. Iterate through the array.
3. If the element is already in the set, return it as the duplicate.
4. If the element is not in the set, add it to the set.

#### Example:
```javascript
function findDuplicate(arr) {
    let seen = new Set();
    for (let num of arr) {
        if (seen.has(num)) {
            return num;
        }
        seen.add(num);
    }
    return null;
}

// Example usage
console.log(findDuplicate([1, 2, 3, 4, 5, 3])); // Output: 3
console.log(findDuplicate([1, 2, 3, 4, 5])); // Output: null
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


