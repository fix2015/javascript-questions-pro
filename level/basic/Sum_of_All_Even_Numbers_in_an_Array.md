## [Sum of All Even Numbers in an Array](#sum-of-all-even-numbers-in-an-array)

### Sum of All Even Numbers in an Array

To find the sum of all even numbers in an array, iterate through the array and add the even numbers to a running total.

#### Algorithm:
1. Initialize a variable to store the sum of even numbers.
2. Iterate through the array and check if each number is even (i.e., divisible by 2).
3. If the number is even, add it to the sum.
4. Return the final sum.

#### Example:
```javascript
function sumEvenNumbers(arr) {
    let sum = 0;
    for (const num of arr) {
        if (num % 2 === 0) {
            sum += num;
        }
    }
    return sum;
}

// Example usage
console.log(sumEvenNumbers([1, 2, 3, 4, 5, 6])); // Output: 12
console.log(sumEvenNumbers([10, 15, 20, 25])); // Output: 30
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


