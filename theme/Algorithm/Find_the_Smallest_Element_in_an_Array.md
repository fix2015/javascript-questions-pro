## [Find the Smallest Element in an Array](#find-the-smallest-element-in-an-array)

### Find the Smallest Element in an Array

To find the smallest element in an array, iterate through the array and keep track of the smallest element.

#### Algorithm:
1. Initialize a variable to store the smallest element with a large value (e.g., `Infinity`).
2. Iterate through the array and compare each element to the current smallest value.
3. Update the smallest value whenever a smaller element is found.
4. Return the smallest value.

#### Example:
```javascript
function findSmallest(arr) {
    let smallest = Infinity;

    for (const num of arr) {
        if (num < smallest) {
            smallest = num;
        }
    }

    return smallest;
}

// Example usage
console.log(findSmallest([5, 3, 8, 1, 6])); // Output: 1
console.log(findSmallest([7, 4, 9, 2])); // Output: 2
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


