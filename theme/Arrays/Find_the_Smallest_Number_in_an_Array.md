## [Find the Smallest Number in an Array](#find-the-smallest-number-in-an-array)

### Find the Smallest Number in an Array

To find the smallest number in an array, iterate through the array and keep track of the smallest value encountered.

#### Algorithm:
1. Initialize a variable to store the smallest value, starting with the first element of the array.
2. Iterate through the array and compare each element with the current smallest value.
3. If an element is smaller than the current smallest, update the smallest value.
4. Return the smallest value after completing the iteration.

#### Example:
```javascript
function findSmallestNumber(arr) {
    if (arr.length === 0) {
        throw new Error('Array is empty');
    }

    let smallest = arr[0];

    for (const num of arr) {
        if (num < smallest) {
            smallest = num;
        }
    }

    return smallest;
}

// Example usage
console.log(findSmallestNumber([3, 1, 4, 1, 5, 9])); // Output: 1
console.log(findSmallestNumber([-10, -20, -3, -7])); // Output: -20
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


