## [Find the Longest Common Prefix](#find-the-longest-common-prefix)

### Find the Longest Common Prefix

To find the longest common prefix among a set of strings, iterate through the strings character by character and check if they match.

#### Algorithm:
1. Sort the array of strings.
2. Compare the first and the last string character by character.
3. The characters that match are the common prefix.
4. Return the common prefix.

#### Example:
```javascript
function longestCommonPrefix(strs) {
    if (strs.length === 0) return '';
    strs.sort();
    let first = strs[0], last = strs[strs.length - 1];
    let i = 0;
    while (i < first.length && first[i] === last[i]) {
        i++;
    }
    return first.substring(0, i);
}

// Example usage
console.log(longestCommonPrefix(['flower', 'flow', 'flight'])); // Output: 'fl'
console.log(longestCommonPrefix(['dog', 'racecar', 'car'])); // Output: ''
```

This method has a time complexity of O(n log n), where n is the number of strings.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


