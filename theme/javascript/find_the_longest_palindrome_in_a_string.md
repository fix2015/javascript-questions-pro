## [Find the Longest Palindrome in a String](#find-the-longest-palindrome-in-a-string)

### Find the Longest Palindrome in a String

To find the longest palindrome in a string, expand around each character and check for the longest palindromic substring.

#### Algorithm:
1. Initialize variables to store the start and end indices of the longest palindrome.
2. For each character in the string, expand outwards while the characters on both sides match.
3. Track the maximum length of palindrome found during the expansion.
4. Return the longest palindromic substring.

#### Example:
```javascript
function longestPalindrome(s) {
    let start = 0, end = 0;
    for (let i = 0; i < s.length; i++) {
        let len1 = expandAroundCenter(s, i, i);
        let len2 = expandAroundCenter(s, i, i + 1);
        let len = Math.max(len1, len2);
        if (len > (end - start)) {
            start = i - Math.floor((len - 1) / 2);
            end = i + Math.floor(len / 2);
        }
    }
    return s.substring(start, end + 1);
}

function expandAroundCenter(s, left, right) {
    while (left >= 0 && right < s.length && s[left] === s[right]) {
        left--;
        right++;
    }
    return right - left - 1;
}

// Example usage
console.log(longestPalindrome('babad')); // Output: 'bab' or 'aba'
console.log(longestPalindrome('cbbd')); // Output: 'bb'
```

This method has a time complexity of O(n^2), where n is the length of the string.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)


