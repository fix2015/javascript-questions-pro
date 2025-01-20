## [Find the First Missing Positive Integer](#find-the-first-missing-positive-integer)

### Find the First Missing Positive Integer

To find the first missing positive integer in an unsorted array, use an in-place hash set technique to rearrange the elements and identify the missing number.

#### Algorithm:
1. Iterate through the array and move each number to its correct position (i.e., `arr[i] = i + 1`).
2. After rearranging, find the first index where the value is not equal to `index + 1`.
3. Return `index + 1` as the first missing positive integer.

#### Example:
```javascript
function firstMissingPositive(nums) {
    for (let i = 0; i < nums.length; i++) {
        while (nums[i] > 0 && nums[i] <= nums.length && nums[nums[i] - 1] !== nums[i]) {
            [nums[nums[i] - 1], nums[i]] = [nums[i], nums[nums[i] - 1]];
        }
    }
    for (let i = 0; i < nums.length; i++) {
        if (nums[i] !== i + 1) return i + 1;
    }
    return nums.length + 1;
}

// Example usage
console.log(firstMissingPositive([1, 2, 0])); // Output: 3
console.log(firstMissingPositive([3, 4, -1, 1])); // Output: 2
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


