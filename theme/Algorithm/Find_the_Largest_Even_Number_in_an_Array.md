## [Find the Largest Even Number in an Array](#find-the-largest-even-number-in-an-array)

### Find the Largest Even Number in an Array

To find the largest even number in an array, iterate through the array and check each element for evenness, keeping track of the largest even number.

#### Algorithm:
1. Initialize a variable to store the largest even number, starting with a value like `-Infinity`.
2. Iterate through the array and check if each element is even.
3. If the element is even and larger than the current largest even number, update the largest even number.
4. Return the largest even number.

#### Example:
```javascript
function findLargestEven(arr) {
    let largestEven = -Infinity;

    for (const num of arr) {
        if (num % 2 === 0 && num > largestEven) {
            largestEven = num;
        }
    }

    return largestEven === -Infinity ? null : largestEven;
}

// Example usage
console.log(findLargestEven([1, 2, 3, 4, 5])); // Output: 4
console.log(findLargestEven([7, 5, 9, 1])); // Output: null
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


