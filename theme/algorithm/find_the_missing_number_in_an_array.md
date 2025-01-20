## [Find the Missing Number in an Array](#find-the-missing-number-in-an-array)

### Find the Missing Number in an Array

To find the missing number in an array that contains all numbers from 1 to n except one, you can use the sum formula of an arithmetic series.

#### Algorithm:
1. Calculate the expected sum of the numbers from 1 to n using the formula `n * (n + 1) / 2`.
2. Calculate the actual sum of the elements in the array.
3. Subtract the actual sum from the expected sum to find the missing number.

#### Example:
```javascript
function findMissingNumber(arr) {
    let n = arr.length + 1;
    let expectedSum = (n * (n + 1)) / 2;
    let actualSum = arr.reduce((sum, num) => sum + num, 0);
    return expectedSum - actualSum;
}

// Example usage
console.log(findMissingNumber([1, 2, 4, 5])); // Output: 3
console.log(findMissingNumber([1, 3, 4, 5])); // Output: 2
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


