## [Find the Common Elements Between Two Arrays](#find-the-common-elements-between-two-arrays)

### Find the Common Elements Between Two Arrays

To find common elements between two arrays, use a set to store the elements of one array and check for intersections with the other array.

#### Algorithm:
1. Convert the first array into a set.
2. Iterate through the second array and check if each element exists in the set.
3. If it does, add it to the result array.
4. Return the result array.

#### Example:
```javascript
function findCommonElements(arr1, arr2) {
    const set1 = new Set(arr1);
    const common = [];

    for (const num of arr2) {
        if (set1.has(num)) {
            common.push(num);
        }
    }

    return common;
}

// Example usage
console.log(findCommonElements([1, 2, 3], [3, 4, 5])); // Output: [3]
console.log(findCommonElements(["a", "b", "c"], ["d", "b", "e"])); // Output: ["b"]
```

This method has a time complexity of O(n + m), where n and m are the lengths of the two arrays.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


