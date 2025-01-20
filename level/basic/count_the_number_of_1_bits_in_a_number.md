## [Count the Number of 1 Bits in a Number](#count-the-number-of-1-bits-in-a-number)

### Count the Number of 1 Bits in a Number

To count the number of 1 bits in a number, use bitwise operations. The idea is to repeatedly clear the least significant 1 bit and count how many times this operation is performed.

#### Algorithm:
1. Initialize a counter variable to 0.
2. Repeatedly perform the operation `n & (n - 1)` to clear the least significant 1 bit of `n`.
3. Increment the counter for each operation.
4. Return the counter.

#### Example:
```javascript
function hammingWeight(n) {
    let count = 0;
    while (n !== 0) {
        n &= (n - 1);
        count++;
    }
    return count;
}

// Example usage
console.log(hammingWeight(11)); // Output: 3 (binary: 1011)
console.log(hammingWeight(128)); // Output: 1 (binary: 10000000)
```

This method has a time complexity of O(k), where k is the number of 1 bits in the number.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Bit Manipulation](./theme/bit_manipulation), [Algorithm](./theme/algorithm)


