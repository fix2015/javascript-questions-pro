## [Find the Kth Largest Element in an Array](#find-the-kth-largest-element-in-an-array)

### Find the Kth Largest Element in an Array

To find the Kth largest element in an array, you can sort the array in descending order and return the element at the Kth position.

#### Algorithm:
1. Sort the array in descending order.
2. Return the element at index K-1.
3. If K is larger than the length of the array, return `null`.

#### Example:
```javascript
function findKthLargest(arr, k) {
    arr.sort((a, b) => b - a);
    return arr[k - 1] || null;
}

// Example usage
console.log(findKthLargest([1, 3, 5, 2, 4], 2)); // Output: 4
console.log(findKthLargest([7, 2, 9, 4], 3)); // Output: 4
```

This method has a time complexity of O(n log n), where n is the length of the array due to sorting.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


