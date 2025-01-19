## [Find the Second Smallest Number in an Array](#find-the-second-smallest-number-in-an-array)

### Find the Second Smallest Number in an Array

To find the second smallest number in an array, iterate through the array while keeping track of the smallest and second smallest values.

#### Algorithm:
1. Initialize two variables to store the smallest and second smallest values, starting with `Infinity`.
2. Iterate through the array and update the smallest and second smallest values as you go.
3. Return the second smallest number.

#### Example:
```javascript
function findSecondSmallest(arr) {
    let smallest = Infinity;
    let secondSmallest = Infinity;

    for (const num of arr) {
        if (num < smallest) {
            secondSmallest = smallest;
            smallest = num;
        } else if (num < secondSmallest && num > smallest) {
            secondSmallest = num;
        }
    }

    return secondSmallest === Infinity ? null : secondSmallest;
}

// Example usage
console.log(findSecondSmallest([5, 3, 8, 1, 6])); // Output: 3
console.log(findSecondSmallest([1, 1, 1])); // Output: null
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


