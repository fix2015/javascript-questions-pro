## [Find All Prime Numbers in a Range](#find-all-prime-numbers-in-a-range)

### Find All Prime Numbers in a Range

To find all prime numbers within a given range, use the Sieve of Eratosthenes algorithm to efficiently find primes.

#### Algorithm:
1. Create a boolean array `isPrime` where each index represents a number.
2. Set all values to `true` except for 0 and 1.
3. Starting from 2, mark all multiples of each prime as `false`.
4. Return the indices that are still `true` as the prime numbers.

#### Example:
```javascript
function sieveOfEratosthenes(limit) {
    let isPrime = new Array(limit + 1).fill(true);
    isPrime[0] = isPrime[1] = false;
    for (let i = 2; i * i <= limit; i++) {
        if (isPrime[i]) {
            for (let j = i * i; j <= limit; j += i) {
                isPrime[j] = false;
            }
        }
    }
    return isPrime.map((prime, index) => prime ? index : -1).filter(index => index !== -1);
}

// Example usage
console.log(sieveOfEratosthenes(20)); // Output: [2, 3, 5, 7, 11, 13, 17, 19]
```

This method has a time complexity of O(n log log n), where n is the limit.

**Tags**: basic, JavaScript, Math, Algorithm


