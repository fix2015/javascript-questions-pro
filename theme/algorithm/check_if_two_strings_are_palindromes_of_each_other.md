## [Check if Two Strings Are Palindromes of Each Other](#check-if-two-strings-are-palindromes-of-each-other)

### Check if Two Strings Are Palindromes of Each Other

To check if two strings are palindromes of each other, reverse one string and compare it with the other string.

#### Algorithm:
1. Reverse one of the strings.
2. Compare the reversed string with the other string.
3. If they are equal, return true, indicating that they are palindromes of each other.

#### Example:
```javascript
function arePalindromes(str1, str2) {
    return str1 === str2.split('').reverse().join('');
}

// Example usage
console.log(arePalindromes('abcd', 'dcba')); // Output: true
console.log(arePalindromes('abc', 'def')); // Output: false
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


