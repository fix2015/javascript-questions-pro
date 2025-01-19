## [Find the Largest Palindrome in an Array](#find-the-largest-palindrome-in-an-array)

### Find the Largest Palindrome in an Array

To find the largest palindrome in an array, iterate through the array and check if each number is a palindrome, keeping track of the largest one.

#### Algorithm:
1. Iterate through the array and check if each element is a palindrome.
2. For each palindrome, compare it with the current largest palindrome.
3. Return the largest palindrome found.

#### Example:
```javascript
function isPalindrome(num) {
    return num.toString() === num.toString().split('').reverse().join('');
}

function findLargestPalindrome(arr) {
    let largest = -Infinity;
    for (let num of arr) {
        if (isPalindrome(num) && num > largest) {
            largest = num;
        }
    }
    return largest === -Infinity ? 'No palindrome found' : largest;
}

// Example usage
console.log(findLargestPalindrome([121, 123, 232, 456])); // Output: 232
console.log(findLargestPalindrome([123, 456, 789])); // Output: No palindrome found
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


