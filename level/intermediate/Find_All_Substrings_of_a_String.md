## [Find All Substrings of a String](#find-all-substrings-of-a-string)

### Find All Substrings of a String

To find all substrings of a string, iterate through all possible starting and ending indices to extract substrings.

#### Algorithm:
1. Initialize an empty array to store substrings.
2. Iterate through the string with two nested loops: one for the starting index and one for the ending index.
3. Extract the substring for each pair of indices and add it to the result array.
4. Return the array of substrings.

#### Example:
```javascript
function findAllSubstrings(str) {
    const substrings = [];
    for (let i = 0; i < str.length; i++) {
        for (let j = i + 1; j <= str.length; j++) {
            substrings.push(str.slice(i, j));
        }
    }
    return substrings;
}

// Example usage
console.log(findAllSubstrings('abc')); // Output: ['a', 'ab', 'abc', 'b', 'bc', 'c']
console.log(findAllSubstrings('hello')); // Output: ['h', 'he', 'hel', 'hell', 'hello', 'e', 'el', 'ell', 'ello', 'l', 'll', 'llo', 'l', 'lo', 'o']
```

This method has a time complexity of O(n^2), where n is the length of the string.

**Tags**: intermediate, JavaScript, Strings, Algorithm


