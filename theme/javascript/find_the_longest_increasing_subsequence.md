## [Find the Longest Increasing Subsequence](#find-the-longest-increasing-subsequence)

### Find the Longest Increasing Subsequence

The longest increasing subsequence (LIS) is a subsequence of a given array where the elements are in strictly increasing order. The goal is to find the length of the LIS.

#### Algorithm:
1. Initialize an array `dp` where `dp[i]` stores the length of the longest increasing subsequence that ends at index `i`.
2. Iterate through the array, and for each element, check all previous elements to see if it can form a longer subsequence.
3. Return the maximum value in `dp`.

#### Example:
```javascript
function lengthOfLIS(nums) {
    if (nums.length === 0) return 0;
    let dp = new Array(nums.length).fill(1);
    for (let i = 1; i < nums.length; i++) {
        for (let j = 0; j < i; j++) {
            if (nums[i] > nums[j]) {
                dp[i] = Math.max(dp[i], dp[j] + 1);
            }
        }
    }
    return Math.max(...dp);
}

// Example usage
console.log(lengthOfLIS([10, 9, 2, 5, 3, 7, 101, 18])); // Output: 4
```

This method has a time complexity of O(n^2), where n is the length of the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


