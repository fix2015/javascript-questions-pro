## [Find the Majority Element](#find-the-majority-element)

### Find the Majority Element

The majority element in an array is the element that appears more than `n/2` times. The Boyer-Moore Voting Algorithm is an efficient way to find this element.

#### Algorithm:
1. Initialize a candidate element and a count variable.
2. Iterate through the array, updating the count based on the current element.
3. If the count becomes 0, set the current element as the new candidate.
4. After the first pass, the candidate will be the majority element if it exists.

#### Example:
```javascript
function majorityElement(arr) {
    let candidate = null;
    let count = 0;
    for (let num of arr) {
        if (count === 0) {
            candidate = num;
        }
        count += (num === candidate) ? 1 : -1;
    }
    return candidate;
}

// Example usage
console.log(majorityElement([3, 3, 4, 2, 4, 4, 2, 4, 4])); // Output: 4
console.log(majorityElement([1, 2, 3, 4, 5])); // Output: 5 (or no majority)
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


