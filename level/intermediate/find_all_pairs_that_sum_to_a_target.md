## [Find All Pairs That Sum to a Target](#find-all-pairs-that-sum-to-a-target)

### Find All Pairs That Sum to a Target

To find all pairs of numbers in an array that sum up to a target value, use a hash set to track the numbers seen so far and check if the complement of each number exists in the set.

#### Algorithm:
1. Initialize an empty set to store the numbers.
2. Iterate through the array and for each number, check if the complement (target - number) is already in the set.
3. If the complement exists, add the pair to the result array.
4. If the complement doesn't exist, add the current number to the set.

#### Example:
```javascript
function findPairs(arr, target) {
    let pairs = [];
    let seen = new Set();
    for (let num of arr) {
        let complement = target - num;
        if (seen.has(complement)) {
            pairs.push([complement, num]);
        }
        seen.add(num);
    }
    return pairs;
}

// Example usage
console.log(findPairs([1, 2, 3, 4, 5], 5)); // Output: [[2, 3], [1, 4]]
console.log(findPairs([1, 3, 2, 4, 5], 6)); // Output: [[1, 5], [2, 4]]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


