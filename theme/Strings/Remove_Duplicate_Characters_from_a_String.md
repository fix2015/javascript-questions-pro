## [Remove Duplicate Characters from a String](#remove-duplicate-characters-from-a-string)

### Remove Duplicate Characters from a String

To remove duplicate characters from a string, you can use a set to store unique characters.

#### Algorithm:
1. Initialize an empty set to store unique characters.
2. Iterate through the string and add each character to the set.
3. Join the characters from the set into a new string and return it.

#### Example:
```javascript
function removeDuplicates(str) {
    return [...new Set(str)].join('');
}

// Example usage
console.log(removeDuplicates("programming")); // Output: "progamin"
console.log(removeDuplicates("hello")); // Output: "helo"
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: basic, JavaScript, Strings, Algorithm


