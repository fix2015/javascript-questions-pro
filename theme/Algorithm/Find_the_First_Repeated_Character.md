## [Find the First Repeated Character](#find-the-first-repeated-character)

### Find the First Repeated Character

To find the first repeated character in a string, use a frequency counter to track character occurrences.

#### Algorithm:
1. Initialize an empty set to track characters as you iterate through the string.
2. For each character, check if it already exists in the set.
3. If it does, return the character as the first repeated character.
4. If no repeated character is found, return `null`.

#### Example:
```javascript
function findFirstRepeatedChar(str) {
    const seen = new Set();

    for (const char of str) {
        if (seen.has(char)) {
            return char;
        }
        seen.add(char);
    }

    return null;
}

// Example usage
console.log(findFirstRepeatedChar("abcdab")); // Output: "a"
console.log(findFirstRepeatedChar("abcdef")); // Output: null
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


