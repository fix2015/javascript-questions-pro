## [Find the Largest Sum of Consecutive Subarray](#find-the-largest-sum-of-consecutive-subarray)

### Find the Largest Sum of Consecutive Subarray

To find the largest sum of a consecutive subarray, you can use Kadane's Algorithm.

#### Algorithm:
1. Initialize two variables: `maxSum` and `currentSum`, both set to the first element of the array.
2. Iterate through the array, updating `currentSum` to the larger of the current element or the sum of `currentSum` and the current element.
3. Update `maxSum` to the larger of `maxSum` and `currentSum`.
4. Return `maxSum`.

#### Example:
```javascript
function maxSubArraySum(arr) {
    let maxSum = arr[0], currentSum = arr[0];

    for (let i = 1; i < arr.length; i++) {
        currentSum = Math.max(arr[i], currentSum + arr[i]);
        maxSum = Math.max(maxSum, currentSum);
    }

    return maxSum;
}

// Example usage
console.log(maxSubArraySum([1, -2, 3, 4, -1, 2, 1, -5, 4])); // Output: 7
console.log(maxSubArraySum([-2, -3, 4, -1, -2, 1, 5, -3])); // Output: 7
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


