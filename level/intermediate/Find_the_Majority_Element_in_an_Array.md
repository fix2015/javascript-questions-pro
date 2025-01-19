## [Find the Majority Element in an Array](#find-the-majority-element-in-an-array)

### Find the Majority Element in an Array

To find the majority element in an array (an element that appears more than n/2 times), use the Boyer-Moore Voting Algorithm.

#### Algorithm:
1. Initialize a `candidate` variable and a `count` variable.
2. Iterate through the array. If the count is 0, set the current element as the `candidate` and set `count` to 1. If the current element is the `candidate`, increment the count, otherwise decrement it.
3. Return the `candidate`.

#### Example:
```javascript
function majorityElement(nums) {
    let candidate = null, count = 0;
    for (let num of nums) {
        if (count === 0) {
            candidate = num;
        }
        count += (num === candidate) ? 1 : -1;
    }
    return candidate;
}

// Example usage
console.log(majorityElement([3, 2, 3])); // Output: 3
console.log(majorityElement([1, 2, 3, 4])); // Output: null
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


