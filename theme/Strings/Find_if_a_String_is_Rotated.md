## [Find if a String is Rotated](#find-if-a-string-is-rotated)

### Find if a String is Rotated

To check if one string is a rotation of another, concatenate the second string with itself and check if the first string is a substring of the concatenated string.

#### Algorithm:
1. Concatenate the second string with itself.
2. Check if the first string is a substring of the concatenated string.
3. Return true if it is a substring, false otherwise.

#### Example:
```javascript
function isRotated(str1, str2) {
    if (str1.length !== str2.length) return false;
    return (str2 + str2).includes(str1);
}

// Example usage
console.log(isRotated('abc', 'bca')); // Output: true
console.log(isRotated('abc', 'acb')); // Output: false
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: intermediate, JavaScript, Strings, Algorithm


