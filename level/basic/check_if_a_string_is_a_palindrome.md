## [Check if a String is a Palindrome](#check-if-a-string-is-a-palindrome)

### Check if a String is a Palindrome

A palindrome is a word, phrase, or sequence that reads the same backward as forward.

#### Algorithm:
1. Remove all non-alphanumeric characters and convert the string to lowercase to handle case sensitivity.
2. Use two pointers: one starting at the beginning and the other at the end of the string.
3. Compare characters at the two pointers. If they differ, the string is not a palindrome.
4. Move the pointers closer to the center and repeat the comparison.
5. If all characters match, the string is a palindrome.

#### Example:
```javascript
function isPalindrome(str) {
    // Normalize the string: remove non-alphanumeric characters and convert to lowercase
    const cleanStr = str.replace(/[^a-zA-Z0-9]/g, '').toLowerCase();

    let left = 0;
    let right = cleanStr.length - 1;

    while (left < right) {
        if (cleanStr[left] !== cleanStr[right]) {
            return false; // Not a palindrome
        }
        left++;
        right--;
    }

    return true; // It's a palindrome
}

// Example usage
console.log(isPalindrome("A man, a plan, a canal, Panama")); // Output: true
console.log(isPalindrome("hello")); // Output: false
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm)

**URL**: [https://www.tiktok.com/@jsmentoring/video/7458413373315681569](https://www.tiktok.com/@jsmentoring/video/7458413373315681569)
