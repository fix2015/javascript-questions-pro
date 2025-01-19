## [Find the Second Largest Element in an Array](#find-the-second-largest-element-in-an-array)

### Find the Second Largest Element in an Array

To find the second largest element in an array, iterate through the array and keep track of the largest and second largest elements.

#### Algorithm:
1. Initialize two variables, `largest` and `secondLargest`, with a very small value (e.g., `-Infinity`).
2. Iterate through the array, updating `largest` and `secondLargest` as needed.
3. Return the second largest element.

#### Example:
```javascript
function findSecondLargest(arr) {
    let largest = -Infinity, secondLargest = -Infinity;

    for (const num of arr) {
        if (num > largest) {
            secondLargest = largest;
            largest = num;
        } else if (num > secondLargest && num < largest) {
            secondLargest = num;
        }
    }

    return secondLargest;
}

// Example usage
console.log(findSecondLargest([5, 2, 8, 3, 1])); // Output: 5
console.log(findSecondLargest([10, 10, 9, 8])); // Output: 9
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


