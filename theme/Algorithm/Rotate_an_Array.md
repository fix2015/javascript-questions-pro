## [Rotate an Array](#rotate-an-array)

### Rotate an Array

To rotate an array, move the elements from one end to the other by a specified number of positions.

#### Algorithm:
1. Calculate the effective number of rotations by taking the modulus of the length of the array with the rotation count.
2. Slice the array into two parts: the part to be moved and the remaining part.
3. Concatenate the two parts in the rotated order.
4. Return the rotated array.

#### Example:
```javascript
function rotateArray(arr, k) {
    const rotations = k % arr.length;
    return [...arr.slice(rotations), ...arr.slice(0, rotations)];
}

// Example usage
console.log(rotateArray([1, 2, 3, 4, 5], 2)); // Output: [3, 4, 5, 1, 2]
console.log(rotateArray([1, 2, 3], 4)); // Output: [2, 3, 1]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


