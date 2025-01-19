## [How do you find min and max values without Math functions](#how-do-you-find-min-and-max-values-without-math-functions)

### How do you find min and max values without Math functions?

You can find the minimum and maximum values in an array by manually iterating over the array and comparing each element.

Example:

```javascript
const arr = [1, 2, 3, 4, 5];
let min = arr[0], max = arr[0];
for (let i = 1; i < arr.length; i++) {
  if (arr[i] < min) min = arr[i];
  if (arr[i] > max) max = arr[i];
}
console.log(min); // 1
console.log(max); // 5
```

**Tags**: basic, JavaScript, arrays


