## [Find the Second Largest Number in an Array](#find-the-second-largest-number-in-an-array)

### Find the Second Largest Number in an Array

To find the second largest number in an array, iterate through the array and keep track of the largest and second largest elements.

#### Algorithm:
1. Initialize two variables, `first` and `second`, to `-Infinity`.
2. Iterate through the array, and for each element, check if it is greater than `first`.
3. If it is, update `second` to `first` and then update `first` to the current element.
4. If the element is smaller than `first` but greater than `second`, update `second`.
5. Return `second` as the second largest element.

#### Example:
```javascript
function findSecondLargest(arr) {
    let first = -Infinity, second = -Infinity;
    for (let num of arr) {
        if (num > first) {
            second = first;
            first = num;
        } else if (num > second && num !== first) {
            second = num;
        }
    }
    return second;
}

// Example usage
console.log(findSecondLargest([10, 20, 4, 45, 99])); // Output: 45
console.log(findSecondLargest([1, 1, 1])); // Output: -Infinity
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


