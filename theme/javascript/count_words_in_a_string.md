## [Count Words in a String](#count-words-in-a-string)

### Count Words in a String

To count the number of words in a string, split the string by spaces and count the resulting elements.

#### Algorithm:
1. Split the string by spaces into an array of words.
2. Filter out any empty strings from the array.
3. Return the length of the array.

#### Example:
```javascript
function countWords(str) {
    return str.split(' ').filter(word => word !== '').length;
}

// Example usage
console.log(countWords('Hello world, how are you?')); // Output: 5
console.log(countWords('   This is a test   ')); // Output: 4
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


