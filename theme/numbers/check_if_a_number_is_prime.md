## [Check if a Number is Prime](#check-if-a-number-is-prime)

### Check if a Number is Prime

To check if a number is prime, verify that it is greater than 1 and divisible only by 1 and itself.

#### Algorithm:
1. Check if the number is less than or equal to 1; if so, return false.
2. Iterate through numbers from 2 to the square root of the number.
3. If the number is divisible by any of these, return false.
4. If no divisors are found, return true.

#### Example:
```javascript
function isPrime(num) {
    if (num <= 1) {
        return false;
    }

    for (let i = 2; i <= Math.sqrt(num); i++) {
        if (num % i === 0) {
            return false;
        }
    }

    return true;
}

// Example usage
console.log(isPrime(7)); // Output: true
console.log(isPrime(10)); // Output: false
```

This method has a time complexity of O(sqrt(n)), where n is the number being checked.

**Tags**: basic, JavaScript, Numbers, Algorithm


