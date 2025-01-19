## [Find the First Repeating Character](#find-the-first-repeating-character)

### Find the First Repeating Character

To find the first repeating character in a string, use a set to track characters that have been seen. As you iterate through the string, check if the character is already in the set.

#### Algorithm:
1. Initialize an empty set to track seen characters.
2. Iterate through the string.
3. If a character is already in the set, return it as the first repeating character.
4. If not, add it to the set.

#### Example:
```javascript
function firstRepeatingCharacter(str) {
    let seen = new Set();
    for (let char of str) {
        if (seen.has(char)) {
            return char;
        }
        seen.add(char);
    }
    return null;
}

// Example usage
console.log(firstRepeatingCharacter('abca')); // Output: 'a'
console.log(firstRepeatingCharacter('abcdef')); // Output: null
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: basic, JavaScript, Strings, Algorithm


