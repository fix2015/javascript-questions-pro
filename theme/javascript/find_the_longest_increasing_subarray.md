## [Find the Longest Increasing Subarray](#find-the-longest-increasing-subarray)

### Find the Longest Increasing Subarray

To find the longest increasing subarray, iterate through the array and track the length of the current increasing subarray.

#### Algorithm:
1. Initialize variables to track the current and maximum subarray lengths.
2. Iterate through the array and check if the current element is greater than the previous one.
3. If the current element is greater, increment the current subarray length.
4. If not, compare the current subarray length with the maximum length and reset the current subarray length.
5. Return the maximum subarray length.

#### Example:
```javascript
function longestIncreasingSubarray(arr) {
    let maxLength = 1, currentLength = 1;

    for (let i = 1; i < arr.length; i++) {
        if (arr[i] > arr[i - 1]) {
            currentLength++;
            maxLength = Math.max(maxLength, currentLength);
        } else {
            currentLength = 1;
        }
    }

    return maxLength;
}

// Example usage
console.log(longestIncreasingSubarray([1, 2, 3, 1, 2, 3, 4])); // Output: 4
console.log(longestIncreasingSubarray([5, 4, 3, 2, 1])); // Output: 1
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


