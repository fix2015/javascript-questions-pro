## [Sort an Array in Ascending Order](#sort-an-array-in-ascending-order)

### Sort an Array in Ascending Order

To sort an array in ascending order, you can use the `sort` method in JavaScript.

#### Algorithm:
1. Use the `sort` method with a comparison function to sort the array in ascending order.
2. The comparison function should return a negative, zero, or positive value based on the comparison of two elements.
3. Return the sorted array.

#### Example:
```javascript
function sortArray(arr) {
    return arr.sort((a, b) => a - b);
}

// Example usage
console.log(sortArray([5, 2, 9, 1, 5, 6])); // Output: [1, 2, 5, 5, 6, 9]
console.log(sortArray([3, 1, 4, 2])); // Output: [1, 2, 3, 4]
```

This method has a time complexity of O(n log n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


