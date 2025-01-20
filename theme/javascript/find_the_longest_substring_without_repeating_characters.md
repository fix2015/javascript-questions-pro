## [Find the Longest Substring Without Repeating Characters](#find-the-longest-substring-without-repeating-characters)

### Find the Longest Substring Without Repeating Characters

To find the longest substring without repeating characters, use a sliding window technique with two pointers to track the current substring.

#### Algorithm:
1. Initialize two pointers, one for the start and one for the end of the window.
2. Move the end pointer to expand the window and add characters to a set.
3. If a character is already in the set, move the start pointer to shrink the window and remove the character from the set.
4. Keep track of the maximum window length.
5. Return the maximum length of the substring.

#### Example:
```javascript
function longestSubstring(str) {
    let start = 0, maxLength = 0, seen = new Set();
    for (let end = 0; end < str.length; end++) {
        while (seen.has(str[end])) {
            seen.delete(str[start]);
            start++;
        }
        seen.add(str[end]);
        maxLength = Math.max(maxLength, end - start + 1);
    }
    return maxLength;
}

// Example usage
console.log(longestSubstring('abcabcbb')); // Output: 3
console.log(longestSubstring('bbbbb')); // Output: 1
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


