## [Sum of All Odd Numbers in an Array](#sum-of-all-odd-numbers-in-an-array)

### Sum of All Odd Numbers in an Array

To calculate the sum of all odd numbers in an array, iterate through the array and add up the odd numbers.

#### Algorithm:
1. Initialize a variable to store the sum.
2. Iterate through the array, checking if each number is odd.
3. If the number is odd, add it to the sum.
4. Return the sum.

#### Example:
```javascript
function sumOfOdds(arr) {
    return arr.filter(num => num % 2 !== 0).reduce((sum, num) => sum + num, 0);
}

// Example usage
console.log(sumOfOdds([1, 2, 3, 4, 5])); // Output: 9
console.log(sumOfOdds([6, 7, 8, 9])); // Output: 16
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


