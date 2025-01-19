## [Reverse a String](#reverse-a-string)

### Reverse a String

To reverse a string, you can split the string into an array of characters, reverse the array, and then join the characters back into a string.

#### Algorithm:
1. Convert the string into an array of characters.
2. Use the `reverse()` method to reverse the array.
3. Join the array back into a string using the `join()` method.
4. Return the reversed string.

#### Example:
```javascript
function reverseString(str) {
    return str.split('').reverse().join('');
}

// Example usage
console.log(reverseString("hello")); // Output: "olleh"
console.log(reverseString("JavaScript")); // Output: "tpircSavaJ"
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


