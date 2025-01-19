## [Reverse an Array In-Place](#reverse-an-array-in-place)

### Reverse an Array In-Place

To reverse an array in-place, use two pointers, one at the start and one at the end of the array. Swap elements at these pointers and move towards the center.

#### Algorithm:
1. Initialize two pointers: one at the start and one at the end of the array.
2. Swap the elements at these pointers.
3. Move the pointers towards the center.
4. Repeat until the pointers cross.

#### Example:
```javascript
function reverseArray(arr) {
    let start = 0;
    let end = arr.length - 1;
    while (start < end) {
        [arr[start], arr[end]] = [arr[end], arr[start]];
        start++;
        end--;
    }
    return arr;
}

// Example usage
console.log(reverseArray([1, 2, 3, 4, 5])); // Output: [5, 4, 3, 2, 1]
console.log(reverseArray([10, 20, 30])); // Output: [30, 20, 10]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: basic, JavaScript, Arrays, Algorithm


