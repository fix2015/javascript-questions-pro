## [Find if a Number is Prime](#find-if-a-number-is-prime)

### Find if a Number is Prime

A prime number is a number greater than 1 that has no divisors other than 1 and itself. To check if a number is prime, iterate through numbers from 2 to the square root of the number.

#### Algorithm:
1. If the number is less than or equal to 1, return `false`.
2. Check for divisibility by all numbers from 2 to the square root of the number.
3. If any number divides evenly, return `false`. Otherwise, return `true`.

#### Example:
```javascript
function isPrime(num) {
    if (num <= 1) return false;
    for (let i = 2; i <= Math.sqrt(num); i++) {
        if (num % i === 0) return false;
    }
    return true;
}

// Example usage
console.log(isPrime(7));  // Output: true
console.log(isPrime(10)); // Output: false
```

This method has a time complexity of O(sqrt(n)), where n is the number being checked.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Math](./theme/math), [Algorithm](./theme/algorithm)


