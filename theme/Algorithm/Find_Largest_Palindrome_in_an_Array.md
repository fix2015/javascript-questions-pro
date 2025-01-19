## [Find Largest Palindrome in an Array](#find-largest-palindrome-in-an-array)

### Find Largest Palindrome in an Array

To find the largest palindrome in an array, iterate through the array and check each element to see if it is a palindrome.

#### Algorithm:
1. Iterate through the array and check if each element is a palindrome.
2. Keep track of the largest palindrome found.
3. Return the largest palindrome.

#### Example:
```javascript
function isPalindrome(str) {
    return str === str.split('').reverse().join('');
}

function largestPalindrome(arr) {
    let largest = '';
    for (let str of arr) {
        if (isPalindrome(str) && str.length > largest.length) {
            largest = str;
        }
    }
    return largest;
}

// Example usage
console.log(largestPalindrome(['madam', 'racecar', 'apple'])); // Output: 'racecar'
console.log(largestPalindrome(['hello', 'world', 'civic'])); // Output: 'civic'
```

This method has a time complexity of O(n * m), where n is the length of the array and m is the average length of the strings.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


