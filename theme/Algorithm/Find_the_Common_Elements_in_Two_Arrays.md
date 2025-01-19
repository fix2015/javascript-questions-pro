## [Find the Common Elements in Two Arrays](#find-the-common-elements-in-two-arrays)

### Find the Common Elements in Two Arrays

To find the common elements in two arrays, you can use a set to track elements from one array and check if they exist in the other array.

#### Algorithm:
1. Create a set from the first array to store unique elements.
2. Iterate through the second array and check if each element is present in the set.
3. If an element is found in both arrays, add it to the result array.
4. Return the array of common elements.

#### Example:
```javascript
function findCommonElements(arr1, arr2) {
    const set1 = new Set(arr1);
    const common = [];

    for (const elem of arr2) {
        if (set1.has(elem)) {
            common.push(elem);
        }
    }

    return common;
}

// Example usage
console.log(findCommonElements([1, 2, 3], [2, 3, 4])); // Output: [2, 3]
console.log(findCommonElements(["apple", "banana"], ["banana", "orange"])); // Output: ["banana"]
```

This method has a time complexity of O(n + m), where n and m are the lengths of the two arrays.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


