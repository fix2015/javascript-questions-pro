## [Count the Occurrences of an Element in an Array](#count-the-occurences-of-an-element-in-an-array)

### Count the Occurrences of an Element in an Array

To count the occurrences of an element in an array, iterate through the array and keep track of how many times the element appears.

#### Algorithm:
1. Initialize a counter variable to 0.
2. Iterate through the array and check if each element matches the target element.
3. Increment the counter for each match.
4. Return the counter.

#### Example:
```javascript
function countOccurrences(arr, elem) {
    let count = 0;

    for (const item of arr) {
        if (item === elem) {
            count++;
        }
    }

    return count;
}

// Example usage
console.log(countOccurrences([1, 2, 3, 2, 4], 2)); // Output: 2
console.log(countOccurrences(["apple", "banana", "apple"], "apple")); // Output: 2
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


