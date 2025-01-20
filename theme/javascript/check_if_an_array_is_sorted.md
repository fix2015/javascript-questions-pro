## [Check if an Array is Sorted](#check-if-an-array-is-sorted)

### Check if an Array is Sorted

To check if an array is sorted, compare each element with the next one to ensure it is in the correct order.

#### Algorithm:
1. Iterate through the array and compare each element with the next.
2. If any element is greater than the next one, the array is not sorted.
3. If no such element is found, return true; otherwise, return false.

#### Example:
```javascript
function isArraySorted(arr) {
    for (let i = 0; i < arr.length - 1; i++) {
        if (arr[i] > arr[i + 1]) {
            return false;
        }
    }
    return true;
}

// Example usage
console.log(isArraySorted([1, 2, 3, 4])); // Output: true
console.log(isArraySorted([1, 3, 2, 4])); // Output: false
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


