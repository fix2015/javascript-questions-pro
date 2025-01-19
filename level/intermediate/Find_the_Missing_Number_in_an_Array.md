## [Find the Missing Number in an Array](#find-missing-number-in-an-array)

### Find the Missing Number in an Array

To find the missing number in a sequential array, calculate the expected sum and subtract the actual sum of the array.

#### Algorithm:
1. Calculate the sum of numbers from 1 to n using the formula `n * (n + 1) / 2`.
2. Calculate the sum of the elements in the array.
3. Subtract the actual sum from the expected sum to find the missing number.

#### Example:
```javascript
function findMissingNumber(arr) {
    const n = arr.length + 1;
    const expectedSum = (n * (n + 1)) / 2;
    const actualSum = arr.reduce((sum, num) => sum + num, 0);

    return expectedSum - actualSum;
}

// Example usage
console.log(findMissingNumber([1, 2, 4, 5, 6])); // Output: 3
console.log(findMissingNumber([3, 7, 1, 2, 8, 4, 5])); // Output: 6
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


