## [Find the Largest Sum of Contiguous Subarray](#find-the-largest-sum-of-contiguous-subarray)

### Find the Largest Sum of Contiguous Subarray

To find the largest sum of a contiguous subarray, use Kadane's Algorithm, which helps to find the maximum sum efficiently in linear time.

#### Algorithm:
1. Initialize two variables, `maxCurrent` and `maxGlobal`, to the first element of the array.
2. Iterate through the array starting from the second element.
3. For each element, update `maxCurrent` to the maximum of the current element or the sum of the current element and `maxCurrent`.
4. If `maxCurrent` exceeds `maxGlobal`, update `maxGlobal`.
5. Return `maxGlobal` as the result.

#### Example:
```javascript
function maxSubArraySum(arr) {
    let maxCurrent = maxGlobal = arr[0];
    for (let i = 1; i < arr.length; i++) {
        maxCurrent = Math.max(arr[i], maxCurrent + arr[i]);
        if (maxCurrent > maxGlobal) {
            maxGlobal = maxCurrent;
        }
    }
    return maxGlobal;
}

// Example usage
console.log(maxSubArraySum([1, -2, 3, 4, -1, 2, 1, -5, 4])); // Output: 7
console.log(maxSubArraySum([-1, -2, -3, -4])); // Output: -1
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


