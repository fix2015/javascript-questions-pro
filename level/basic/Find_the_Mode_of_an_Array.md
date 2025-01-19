## [Find the Mode of an Array](#find-the-mode-of-an-array)

### Find the Mode of an Array

To find the mode (most frequent element) of an array, use an object to count the occurrences of each element.

#### Algorithm:
1. Initialize an empty object to store counts of elements.
2. Iterate through the array, updating the count for each element.
3. Find the element with the highest count.
4. Return the element with the highest frequency.

#### Example:
```javascript
function findMode(arr) {
    const counts = {};
    let maxCount = 0;
    let mode = null;

    for (let num of arr) {
        counts[num] = (counts[num] || 0) + 1;
        if (counts[num] > maxCount) {
            maxCount = counts[num];
            mode = num;
        }
    }

    return mode;
}

// Example usage
console.log(findMode([1, 2, 3, 3, 4, 5])); // Output: 3
console.log(findMode([10, 10, 10, 5, 5, 1])); // Output: 10
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


