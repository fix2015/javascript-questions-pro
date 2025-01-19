## [Find the Largest Number in an Array](#find-the-largest-number-in-an-array)

### Find the Largest Number in an Array

To find the largest number in an array, iterate through the array and keep track of the largest number.

#### Algorithm:
1. Initialize a variable to store the largest number with a small value (e.g., `-Infinity`).
2. Iterate through the array and compare each element to the current largest number.
3. Update the largest number whenever a larger element is found.
4. Return the largest number.

#### Example:
```javascript
function findLargest(arr) {
    let largest = -Infinity;

    for (const num of arr) {
        if (num > largest) {
            largest = num;
        }
    }

    return largest;
}

// Example usage
console.log(findLargest([5, 3, 8, 1, 6])); // Output: 8
console.log(findLargest([7, 4, 9, 2])); // Output: 9
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


