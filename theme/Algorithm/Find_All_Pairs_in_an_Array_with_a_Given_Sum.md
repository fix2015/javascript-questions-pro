## [Find All Pairs in an Array with a Given Sum](#find-all-pairs-in-an-array-with-a-given-sum)

### Find All Pairs in an Array with a Given Sum

To find all pairs that sum to a specific target, use a hash set to track the complements of each element.

#### Algorithm:
1. Initialize an empty set to store elements.
2. Iterate through the array and calculate the complement (target - current element).
3. If the complement exists in the set, add the pair to the result.
4. Otherwise, add the current element to the set.
5. Return the list of pairs.

#### Example:
```javascript
function findPairsWithSum(arr, target) {
    const seen = new Set(), pairs = [];
    for (let num of arr) {
        const complement = target - num;
        if (seen.has(complement)) {
            pairs.push([complement, num]);
        }
        seen.add(num);
    }
    return pairs;
}

// Example usage
console.log(findPairsWithSum([1, 2, 3, 4, 5], 5)); // Output: [[2, 3], [1, 4]]
console.log(findPairsWithSum([10, 15, 3, 7], 17)); // Output: [[10, 7]]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


