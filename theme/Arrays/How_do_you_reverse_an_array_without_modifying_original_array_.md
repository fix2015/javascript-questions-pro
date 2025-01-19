## [How do you reverse an array without modifying original array?](#how-do-you-reverse-an-array-without-modifying-original-array)

### How do you reverse an array without modifying original array?

Use the `slice` method to create a shallow copy and then reverse the copy:

```javascript
const originalArray = [1, 2, 3];
const reversedArray = originalArray.slice().reverse();
console.log(originalArray); // [1, 2, 3]
console.log(reversedArray); // [3, 2, 1]
```

**Tags**: intermediate, JavaScript, Arrays


