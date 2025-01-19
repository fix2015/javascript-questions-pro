## [Find All Pairs with a Given Sum](#find-all-pairs-with-sum)

### Find All Pairs with a Given Sum

To find all pairs in an array that sum up to a specific target value, use a hash set to track the numbers that can form pairs.

#### Algorithm:
1. Initialize an empty set to store numbers.
2. Iterate through the array and for each element, check if the complement (target - current element) is in the set.
3. If the complement exists, add the pair to the result array.
4. If not, add the current element to the set.
5. Return the array of pairs.

#### Example:
```javascript
function findPairs(arr, target) {
    const pairs = [];
    const seen = new Set();
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
console.log(findPairs([1, 2, 3, 4, 5], 5)); // Output: [[1, 4], [2, 3]]
console.log(findPairs([10, 15, 3, 7], 17)); // Output: [[10, 7]]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: intermediate, JavaScript, Arrays, Algorithm


