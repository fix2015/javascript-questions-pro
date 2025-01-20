## [Merge Two Sorted Arrays](#merge-two-sorted-arrays)

### Merge Two Sorted Arrays

To merge two sorted arrays into one sorted array, use two pointers to compare the elements from both arrays.

#### Algorithm:
1. Initialize two pointers, one for each array.
2. Compare the elements at the current pointers and add the smaller element to the result array.
3. Move the pointer of the array from which the element was taken.
4. If one array is exhausted, add the remaining elements of the other array to the result.
5. Return the merged sorted array.

#### Example:
```javascript
function mergeSortedArrays(arr1, arr2) {
    let result = [];
    let i = 0, j = 0;

    while (i < arr1.length && j < arr2.length) {
        if (arr1[i] < arr2[j]) {
            result.push(arr1[i]);
            i++;
        } else {
            result.push(arr2[j]);
            j++;
        }
    }

    return result.concat(arr1.slice(i), arr2.slice(j));
}

// Example usage
console.log(mergeSortedArrays([1, 3, 5], [2, 4, 6])); // Output: [1, 2, 3, 4, 5, 6]
```

This method has a time complexity of O(n + m), where n and m are the lengths of the two arrays.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


