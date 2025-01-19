## [Find the Kth Smallest Element in an Array](#find-the-kth-smallest-element-in-an-array)

### Find the Kth Smallest Element in an Array

To find the Kth smallest element in an array, use the Quickselect algorithm or sort the array and return the element at the Kth index.

#### Algorithm (Quickselect):
1. Select a pivot element from the array.
2. Partition the array into two subarrays: one with elements smaller than the pivot, and one with elements larger.
3. If the Kth element is in the smaller subarray, repeat the process with that subarray.
4. If the Kth element is in the larger subarray, repeat the process with that subarray.
5. Return the Kth smallest element.

#### Example (using sorting):
```javascript
function kthSmallest(arr, k) {
    arr.sort((a, b) => a - b);
    return arr[k - 1];
}

// Example usage
console.log(kthSmallest([7, 10, 4, 3, 20, 15], 4)); // Output: 10
console.log(kthSmallest([12, 3, 5, 7, 19], 2)); // Output: 5
```

This method has a time complexity of O(n log n) for sorting, where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


