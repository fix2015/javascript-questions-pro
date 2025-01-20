## [Find the Most Frequent Element in an Array](#find-the-most-frequent-element-in-an-array)

### Find the Most Frequent Element in an Array

To find the most frequent element in an array, you can use a frequency counter to track occurrences of each element.

#### Algorithm:
1. Create an empty object to store element frequencies.
2. Iterate through the array and count occurrences of each element by updating the object.
3. Keep track of the element with the highest frequency while iterating through the object.
4. Return the element with the highest frequency.

#### Example:
```javascript
function findMostFrequentElement(arr) {
    const frequency = {};
    let maxFreq = 0;
    let mostFrequent = null;

    // Count occurrences of each element
    for (const elem of arr) {
        frequency[elem] = (frequency[elem] || 0) + 1;
        if (frequency[elem] > maxFreq) {
            maxFreq = frequency[elem];
            mostFrequent = elem;
        }
    }

    return mostFrequent;
}

// Example usage
console.log(findMostFrequentElement([1, 3, 2, 1, 4, 1, 3, 3])); // Output: 1
console.log(findMostFrequentElement(["apple", "banana", "apple", "orange", "banana", "apple"])); // Output: "apple"
```

This method has a time complexity of O(n) as it involves a single iteration over the array.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm), [Data Structures](./theme/data_structures)

**URL**: [https://www.tiktok.com/@jsmentoring/video/7458418483282316576](https://www.tiktok.com/@jsmentoring/video/7458418483282316576)
