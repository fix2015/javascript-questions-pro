## [Find the Middle Element of an Array](#find-the-middle-element-of-an-array)

### Find the Middle Element of an Array

To find the middle element of an array, calculate the index of the middle and return the corresponding element.

#### Algorithm:
1. If the array length is odd, the middle element is the element at index `Math.floor(arr.length / 2)`.
2. If the array length is even, you can choose either of the two middle elements.
3. Return the middle element.

#### Example:
```javascript
function findMiddleElement(arr) {
    const middleIndex = Math.floor(arr.length / 2);
    return arr[middleIndex];
}

// Example usage
console.log(findMiddleElement([1, 2, 3, 4, 5])); // Output: 3
console.log(findMiddleElement([10, 20, 30, 40])); // Output: 30
```

This method has a time complexity of O(1), as it directly accesses the middle element.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


