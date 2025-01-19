## [Find the Average of an Array](#find-the-average-of-an-array)

### Find the Average of an Array

To find the average of an array, sum all the elements in the array and then divide the sum by the number of elements.

#### Algorithm:
1. Initialize a variable to store the sum of the array elements.
2. Iterate through the array and add each element to the sum.
3. Divide the sum by the length of the array to get the average.
4. Return the average.

#### Example:
```javascript
function findAverage(arr) {
    let sum = 0;
    for (const num of arr) {
        sum += num;
    }
    return sum / arr.length;
}

// Example usage
console.log(findAverage([1, 2, 3, 4, 5])); // Output: 3
console.log(findAverage([10, 20, 30])); // Output: 20
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


