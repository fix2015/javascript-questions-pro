## [Find the Median of an Array](#find-the-median-of-an-array)

### Find the Median of an Array

To find the median of an array, first sort the array and then find the middle element.

#### Algorithm:
1. Sort the array in ascending order.
2. If the array has an odd length, return the middle element.
3. If the array has an even length, return the average of the two middle elements.

#### Example:
```javascript
function findMedian(arr) {
    arr.sort((a, b) => a - b);
    const mid = Math.floor(arr.length / 2);
    return arr.length % 2 !== 0 ? arr[mid] : (arr[mid - 1] + arr[mid]) / 2;
}

// Example usage
console.log(findMedian([1, 3, 5, 2, 4])); // Output: 3
console.log(findMedian([7, 1, 2, 8])); // Output: 4.5
```

This method has a time complexity of O(n log n), where n is the length of the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


