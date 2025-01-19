## [Remove an Element from an Array](#remove-element-from-an-array)

### Remove an Element from an Array

To remove an element from an array, you can use the `filter` method or manually iterate through the array.

#### Algorithm:
1. Use the `filter` method to create a new array without the specified element.
2. Alternatively, iterate through the array and remove the element manually.
3. Return the modified array.

#### Example:
```javascript
function removeElement(arr, elem) {
    return arr.filter(item => item !== elem);
}

// Example usage
console.log(removeElement([1, 2, 3, 4, 5], 3)); // Output: [1, 2, 4, 5]
console.log(removeElement(["apple", "banana", "orange"], "banana")); // Output: ["apple", "orange"]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


