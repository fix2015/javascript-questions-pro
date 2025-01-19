## [Find the First Repeating Element in an Array](#find-the-first-repeating-element-in-an-array)

### Find the First Repeating Element in an Array

To find the first repeating element in an array, you can use a set to keep track of the elements you've already seen.

#### Algorithm:
1. Initialize an empty set to store the elements.
2. Iterate through the array, checking if each element is in the set.
3. If it is, return the element as the first repeating one.
4. If no repeating element is found, return `null`.

#### Example:
```javascript
function findFirstRepeating(arr) {
    const seen = new Set();

    for (const num of arr) {
        if (seen.has(num)) {
            return num;
        }
        seen.add(num);
    }

    return null;
}

// Example usage
console.log(findFirstRepeating([1, 2, 3, 2, 4])); // Output: 2
console.log(findFirstRepeating([5, 3, 4, 1])); // Output: null
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


