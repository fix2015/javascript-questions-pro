## [Find the Largest Product of Two Numbers in an Array](#find-the-largest-product-of-two-numbers-in-an-array)

### Find the Largest Product of Two Numbers in an Array

To find the largest product of two numbers in an array, iterate through the array while keeping track of the two largest numbers.

#### Algorithm:
1. Initialize two variables, `max1` and `max2`, to negative infinity.
2. Iterate through the array, updating `max1` and `max2` as you find larger numbers.
3. Return the product of `max1` and `max2`.

#### Example:
```javascript
function largestProduct(arr) {
    let max1 = -Infinity, max2 = -Infinity;
    for (let num of arr) {
        if (num > max1) {
            max2 = max1;
            max1 = num;
        } else if (num > max2) {
            max2 = num;
        }
    }
    return max1 * max2;
}

// Example usage
console.log(largestProduct([1, 2, 3, 4, 5])); // Output: 20
console.log(largestProduct([-10, -10, 5, 2])); // Output: 100
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


