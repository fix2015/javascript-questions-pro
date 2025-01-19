## [Check if a Number is Perfect](#check-if-a-number-is-perfect)

### Check if a Number is Perfect

A perfect number is a positive integer that is equal to the sum of its proper divisors (excluding the number itself).

#### Algorithm:
1. Initialize a variable to store the sum of divisors.
2. Iterate from 1 to half of the number.
3. For each divisor, add it to the sum.
4. If the sum equals the original number, return `true`, otherwise return `false`.

#### Example:
```javascript
function isPerfectNumber(num) {
    let sum = 0;
    for (let i = 1; i <= num / 2; i++) {
        if (num % i === 0) sum += i;
    }
    return sum === num;
}

// Example usage
console.log(isPerfectNumber(28)); // Output: true
console.log(isPerfectNumber(6));  // Output: true
console.log(isPerfectNumber(10)); // Output: false
```

This method has a time complexity of O(n), where n is the number being checked.

**Tags**: intermediate, JavaScript, Math, Algorithm


