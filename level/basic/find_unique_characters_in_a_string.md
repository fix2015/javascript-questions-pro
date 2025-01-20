## [Find Unique Characters in a String](#find-unique-characters-in-a-string)

### Find Unique Characters in a String

To find unique characters in a string, you can use a set to keep track of characters you've seen.

#### Algorithm:
1. Initialize an empty set.
2. Iterate through the string and add each character to the set.
3. Return the characters in the set as a string.

#### Example:
```javascript
function findUniqueChars(str) {
    const uniqueChars = new Set(str);
    return [...uniqueChars].join('');
}

// Example usage
console.log(findUniqueChars('aabbcc')); // Output: 'abc'
console.log(findUniqueChars('hello')); // Output: 'helo'
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


