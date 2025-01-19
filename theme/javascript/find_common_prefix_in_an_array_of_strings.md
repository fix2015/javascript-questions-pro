## [Find Common Prefix in an Array of Strings](#find-common-prefix-in-an-array-of-strings)

### Find Common Prefix in an Array of Strings

To find the longest common prefix among an array of strings, compare characters from each string in the array.

#### Algorithm:
1. Initialize the first string in the array as the common prefix.
2. Iterate through the rest of the strings, updating the common prefix by comparing it with each string.
3. If no common prefix is found, return an empty string.
4. Return the final common prefix.

#### Example:
```javascript
function findCommonPrefix(arr) {
    if (arr.length === 0) return "";

    let prefix = arr[0];
    for (let i = 1; i < arr.length; i++) {
        while (arr[i].indexOf(prefix) !== 0) {
            prefix = prefix.slice(0, prefix.length - 1);
            if (prefix === "") return "";
        }
    }
    return prefix;
}

// Example usage
console.log(findCommonPrefix(["flower", "flow", "flight"])); // Output: "fl"
console.log(findCommonPrefix(["dog", "racecar", "car"])); // Output: ""
```

This method has a time complexity of O(n * m), where n is the length of the array and m is the length of the longest string.

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays), [Algorithm](./theme/algorithm)


