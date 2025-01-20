## [Find the Unique Elements in an Array](#find-the-unique-elements-in-an-array)

### Find the Unique Elements in an Array

To find the unique elements in an array (elements that appear only once), you can use a frequency count with the help of an object or a `Map`.

#### Algorithm:
1. Create a frequency map to count the occurrences of each element in the array.
2. Filter the array to return elements that appear only once.
3. Return the filtered result.

#### Example:
```javascript
function findUniqueElements(arr) {
    let frequency = new Map();
    arr.forEach(item => frequency.set(item, (frequency.get(item) || 0) + 1));
    return arr.filter(item => frequency.get(item) === 1);
}

// Example usage
console.log(findUniqueElements([1, 2, 2, 3, 4, 4])); // Output: [1, 3]
console.log(findUniqueElements([5, 6, 7, 5, 6])); // Output: [7]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


