## [Find the First Non-Repeating Character](#find-the-first-non-repeating-character)

### Find the First Non-Repeating Character

To find the first non-repeating character in a string, you can use a frequency counter to track character occurrences.

#### Algorithm:
1. Create an empty object to store character frequencies.
2. Iterate through the string and count occurrences of each character by updating the object.
3. Iterate through the string again and check the frequency of each character in the object.
4. Return the first character with a frequency of 1.
5. If no non-repeating character is found, return `null`.

#### Example:
```javascript
function firstNonRepeatingChar(str) {
    const charCount = {};

    // Count occurrences of each character
    for (const char of str) {
        charCount[char] = (charCount[char] || 0) + 1;
    }

    // Find the first character with a count of 1
    for (const char of str) {
        if (charCount[char] === 1) {
            return char;
        }
    }

    return null; // Return null if no non-repeating character is found
}

// Example usage
console.log(firstNonRepeatingChar("swiss")); // Output: "w"
```

This method has a time complexity of O(n) as it involves two iterations over the string.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings), [Algorithm](./theme/algorithm), [Data Structures](./theme/data_structures)

**URL**: [https://www.tiktok.com/@jsmentoring/video/7458383226621529376](https://www.tiktok.com/@jsmentoring/video/7458383226621529376)
