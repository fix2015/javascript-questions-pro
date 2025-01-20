## [Find the First Repeated Character in a String](#find-the-first-repeated-character-in-a-string)

### Find the First Repeated Character in a String

To find the first repeated character in a string, use a set to track characters that have been seen.

#### Algorithm:
1. Initialize an empty set to store characters.
2. Iterate through the string, checking if each character has already been seen in the set.
3. If a character is found in the set, return it as the first repeated character.
4. If no repeated character is found, return `null`.

#### Example:
```javascript
function findFirstRepeatedCharacter(str) {
    const seen = new Set();
    for (let char of str) {
        if (seen.has(char)) return char;
        seen.add(char);
    }
    return null;
}

// Example usage
console.log(findFirstRepeatedCharacter('abcdeab')); // Output: 'a'
console.log(findFirstRepeatedCharacter('abcdef')); // Output: null
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


