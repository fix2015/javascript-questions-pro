## [What is a rest parameter](#what-is-a-rest-parameter)

### What is a rest parameter?

A rest parameter allows a function to accept an indefinite number of arguments as an array. It is denoted by `...`.

Example:

```javascript
function sum(...numbers) {
  return numbers.reduce((a, b) => a + b, 0);
}
console.log(sum(1, 2, 3, 4)); // 10
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [functions](./theme/functions)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457471528330988832](https://www.tiktok.com/@jsmentoring/photo/7457471528330988832)
