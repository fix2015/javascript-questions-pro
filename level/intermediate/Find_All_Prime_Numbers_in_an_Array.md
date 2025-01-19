## [Find All Prime Numbers in an Array](#find-all-prime-numbers-in-an-array)

### Find All Prime Numbers in an Array

To find all prime numbers in an array, check each number in the array to see if it is prime.

#### Algorithm:
1. Define a helper function `isPrime` to check if a number is prime.
2. Iterate through the array, calling `isPrime` on each element.
3. Collect the prime numbers and return them.

#### Example:
```javascript
function isPrime(num) {
    if (num <= 1) return false;
    for (let i = 2; i <= Math.sqrt(num); i++) {
        if (num % i === 0) return false;
    }
    return true;
}

function findPrimes(arr) {
    return arr.filter(isPrime);
}

// Example usage
console.log(findPrimes([1, 2, 3, 4, 5, 6])); // Output: [2, 3, 5]
console.log(findPrimes([10, 15, 23, 30])); // Output: [23]
```

This method has a time complexity of O(n * sqrt(m)), where n is the length of the array and m is the largest number in the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


