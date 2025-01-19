## [Find Common Characters in Two Strings](#find-common-characters-in-two-strings)

### Find Common Characters in Two Strings

To find common characters in two strings, use a frequency map for each string and compare the characters.

#### Algorithm:
1. Create a frequency map for each string to count the occurrences of each character.
2. Compare the frequency maps to find common characters.
3. Return the list of common characters.

#### Example:
```javascript
function findCommonCharacters(str1, str2) {
    const map1 = {}, map2 = {};
    for (let char of str1) map1[char] = (map1[char] || 0) + 1;
    for (let char of str2) map2[char] = (map2[char] || 0) + 1;
    const common = [];
    for (let char in map1) {
        if (map2[char]) {
            const count = Math.min(map1[char], map2[char]);
            for (let i = 0; i < count; i++) common.push(char);
        }
    }
    return common;
}

// Example usage
console.log(findCommonCharacters('abc', 'cde')); // Output: ['c']
console.log(findCommonCharacters('aabb', 'abcc')); // Output: ['a', 'b']
```

This method has a time complexity of O(n + m), where n and m are the lengths of the two strings.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


