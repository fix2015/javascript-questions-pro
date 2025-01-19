## [Check if a String is Rotated](#check-if-a-string-is-rotated)

### Check if a String is Rotated

To check if one string is a rotation of another, concatenate the first string with itself and check if the second string is a substring of the result.

#### Algorithm:
1. Concatenate the first string with itself.
2. Check if the second string is a substring of the concatenated string.
3. If it is, return `true`; otherwise, return `false`.

#### Example:
```javascript
function isRotated(str1, str2) {
    if (str1.length !== str2.length) return false;
    return (str1 + str1).includes(str2);
}

// Example usage
console.log(isRotated('abcde', 'cdeab')); // Output: true
console.log(isRotated('abcde', 'abced')); // Output: false
```

This method has a time complexity of O(n), where n is the length of the strings.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


