## [Find the Maximum Number in an Array](#find-the-maximum-number-in-an-array)

### Find the Maximum Number in an Array

To find the maximum number in an array, iterate through the array and keep track of the largest value encountered.

#### Algorithm:
1. Initialize a variable to store the maximum value. Start with the first element of the array.
2. Iterate through the array, comparing each element with the current maximum.
3. If an element is greater than the current maximum, update the maximum.
4. Return the maximum value after completing the iteration.

#### Example:
```javascript
function findMaxNumber(arr) {
    if (arr.length === 0) {
        throw new Error("Array is empty");
    }

    let max = arr[0];

    for (const num of arr) {
        if (num > max) {
            max = num;
        }
    }

    return max;
}

// Example usage
console.log(findMaxNumber([3, 1, 4, 1, 5, 9])); // Output: 9
console.log(findMaxNumber([-10, -20, -3, -7])); // Output: -3
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


