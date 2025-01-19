## [Count Vowels in a String](#count-vowels-in-a-string)

### Count Vowels in a String

To count the vowels in a string, iterate through the string and check if each character is a vowel.

#### Algorithm:
1. Normalize the string by converting it to lowercase to handle case insensitivity.
2. Define a set or array containing all vowel characters (`a, e, i, o, u`).
3. Iterate through the string and count characters that match any vowel.
4. Return the total count of vowels.

#### Example:
```javascript
function countVowels(str) {
    const vowels = new Set(['a', 'e', 'i', 'o', 'u']);
    let count = 0;

    for (const char of str.toLowerCase()) {
        if (vowels.has(char)) {
            count++;
        }
    }

    return count;
}

// Example usage
console.log(countVowels("Hello World")); // Output: 3
console.log(countVowels("JavaScript is awesome!")); // Output: 8
```

This method has a time complexity of O(n), where n is the length of the string.

**Tags**: basic, JavaScript, Strings, Algorithm


