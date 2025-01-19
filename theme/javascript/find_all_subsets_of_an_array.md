## [Find All Subsets of an Array](#find-all-subsets-of-an-array)

### Find All Subsets of an Array

To find all subsets of an array, use a bitwise approach. Each element can either be included or excluded from a subset, so there are `2^n` possible subsets.

#### Algorithm:
1. Initialize an empty array to store the subsets.
2. Iterate over the range from 0 to `2^n - 1`.
3. For each number in the range, use its binary representation to decide which elements to include in the subset.
4. Return the array of subsets.

#### Example:
```javascript
function getSubsets(arr) {
    let subsets = [];
    let n = arr.length;
    for (let i = 0; i < (1 << n); i++) {
        let subset = [];
        for (let j = 0; j < n; j++) {
            if (i & (1 << j)) {
                subset.push(arr[j]);
            }
        }
        subsets.push(subset);
    }
    return subsets;
}

// Example usage
console.log(getSubsets([1, 2, 3]));
// Output: [[], [1], [2], [1, 2], [3], [1, 3], [2, 3], [1, 2, 3]]
```

This method has a time complexity of O(2^n), where n is the length of the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


