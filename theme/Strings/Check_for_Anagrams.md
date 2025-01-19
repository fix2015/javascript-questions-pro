## [Check for Anagrams](#check-for-anagrams)

### Check for Anagrams

An anagram is a word or phrase formed by rearranging the letters of another, using all the original letters exactly once.

#### Algorithm:
1. Remove any non-alphanumeric characters and convert both strings to lowercase.
2. Check if the lengths of the two strings are the same. If not, they cannot be anagrams.
3. Count the frequency of each character in the first string.
4. Compare the character counts with the second string by decrementing the counts. If any count becomes negative or mismatches, the strings are not anagrams.

#### Example:
```javascript
function areAnagrams(str1, str2) {
    // Normalize the strings: remove non-alphanumeric characters and convert to lowercase
    const normalize = str => str.replace(/[^a-zA-Z0-9]/g, '').toLowerCase();
    const s1 = normalize(str1);
    const s2 = normalize(str2);

    if (s1.length !== s2.length) {
        return false; // Different lengths mean they can't be anagrams
    }

    const charCount = {};

    // Count characters in the first string
    for (const char of s1) {
        charCount[char] = (charCount[char] || 0) + 1;
    }

    // Compare characters with the second string
    for (const char of s2) {
        if (!charCount[char]) {
            return false; // Character mismatch
        }
        charCount[char]--;
    }

    return true; // Strings are anagrams
}

// Example usage
console.log(areAnagrams("listen", "silent")); // Output: true
console.log(areAnagrams("hello", "world")); // Output: false
```

This method has a time complexity of O(n), where n is the length of the strings.

**Tags**: intermediate, JavaScript, Strings, Algorithm

**URL**: [https://www.tiktok.com/@jsmentoring/video/7458386392272473377](https://www.tiktok.com/@jsmentoring/video/7458386392272473377)
