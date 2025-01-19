## [Check if a String is a Palindromic Permutation](#check-if-a-string-is-palindromic-permutation)

### Check if a String is a Palindromic Permutation

To check if a string is a permutation of a palindrome, the string's characters must appear in pairs (except possibly one character for odd-length strings).

#### Algorithm:
1. Count the frequency of each character in the string.
2. Check how many characters have an odd frequency.
3. If more than one character has an odd frequency, return false; otherwise, return true.

#### Example:
```javascript
function isPalindromicPermutation(str) {
    const freqMap = {};

    for (const char of str) {
        freqMap[char] = (freqMap[char] || 0) + 1;
    }

    let oddCount = 0;
    for (const count of Object.values(freqMap)) {
        if (count % 2 !== 0) {
            oddCount += 1;
        }
    }

    return oddCount <= 1;
}

// Example usage
console.log(isPalindromicPermutation("civic")); // Output: true
console.log(isPalindromicPermutation("ivicc")); // Output: true
console.log(isPalindromicPermutation("hello")); // Output: false
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: intermediate, JavaScript, Strings, Algorithm


