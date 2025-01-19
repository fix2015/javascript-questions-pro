## [Find the Greatest Common Divisor (GCD)](#find-the-greatest-common-divisor)

### Find the Greatest Common Divisor (GCD)

To find the GCD of two numbers, you can use the Euclidean algorithm.

#### Algorithm:
1. If `b` is 0, return `a` as the GCD.
2. Otherwise, call the function recursively with `b` and `a % b` as the arguments.
3. Repeat until the second number becomes 0.

#### Example:
```javascript
function gcd(a, b) {
    if (b === 0) return a;
    return gcd(b, a % b);
}

// Example usage
console.log(gcd(56, 98)); // Output: 14
console.log(gcd(100, 25)); // Output: 25
```

This method has a time complexity of O(log(min(a, b))), where a and b are the two numbers.

**Tags**: intermediate, JavaScript, Math, Algorithm


