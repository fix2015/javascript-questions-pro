## [How does synchronous iteration works](#how-does-synchronous-iteration-works)

### How does synchronous iteration work?

Synchronous iteration means that each iteration of the loop or iterator occurs one after the other. The code execution waits for the current iteration to complete before moving on to the next one. This is the default behavior in most loops like `for`, `while`, and `forEach`.

Example:

```javascript
const arr = [1, 2, 3];
arr.forEach(item => console.log(item)); // Output: 1, 2, 3
```

**Tags**: basic, JavaScript, iteration


