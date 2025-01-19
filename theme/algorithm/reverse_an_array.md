## [Reverse an Array](#reverse-an-array)

### Reverse an Array

To reverse an array, you can use the `reverse` method or iterate through the array manually.

#### Algorithm:
1. Initialize two pointers: one at the beginning and one at the end of the array.
2. Swap the elements at the two pointers.
3. Move the pointers toward the center until they meet.
4. Return the reversed array.

#### Example:
```javascript
function reverseArray(arr) {
    let left = 0, right = arr.length - 1;

    while (left < right) {
        [arr[left], arr[right]] = [arr[right], arr[left]];
        left++;
        right--;
    }
    return arr;
}

// Example usage
console.log(reverseArray([1, 2, 3, 4])); // Output: [4, 3, 2, 1]
console.log(reverseArray(["a", "b", "c"])); // Output: ["c", "b", "a"]
```

This method has a time complexity of O(n), where n is the length of the array.

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


