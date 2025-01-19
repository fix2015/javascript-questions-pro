## [Find the Longest Word in a Sentence](#find-the-longest-word-in-a-sentence)

### Find the Longest Word in a Sentence

To find the longest word in a sentence, split the sentence into words and compare their lengths.

#### Algorithm:
1. Remove any non-alphanumeric characters except spaces to clean the input.
2. Split the sentence into an array of words using spaces as the delimiter.
3. Iterate through the array, keeping track of the longest word encountered.
4. Return the longest word. If there are multiple words of the same length, return the first one encountered.

#### Example:
```javascript
function findLongestWord(sentence) {
    // Normalize the sentence: remove non-alphanumeric characters except spaces
    const words = sentence.replace(/[^a-zA-Z0-9\s]/g, '').split(' ');

    let longestWord = '';

    for (const word of words) {
        if (word.length > longestWord.length) {
            longestWord = word;
        }
    }

    return longestWord;
}

// Example usage
console.log(findLongestWord("The quick brown fox jumps over the lazy dog.")); // Output: "jumps"
console.log(findLongestWord("Hello world!")); // Output: "Hello"
```

This method has a time complexity of O(n), where n is the total number of characters in the sentence.

**Tags**: basic, JavaScript, Strings, Algorithm


