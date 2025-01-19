## [Find the Unique Element in an Array](#find-the-unique-element-in-an-array)

### Find the Unique Element in an Array

To find the unique element in an array, use the XOR operation, as XOR of a number with itself is 0, and XOR of a number with 0 is the number itself.

#### Algorithm:
1. Initialize a variable `unique` to 0.
2. Iterate through the array, applying XOR to each element and the `unique` variable.
3. The result will be the unique element in the array.

#### Example:
```javascript
function findUnique(arr) {
    let unique = 0;
    for (let num of arr) {
        unique ^= num;
    }
    return unique;
}

// Example usage
console.log(findUnique([1, 2, 3, 2, 1])); // Output: 3
console.log(findUnique([4, 4, 5, 5, 6])); // Output: 6
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


