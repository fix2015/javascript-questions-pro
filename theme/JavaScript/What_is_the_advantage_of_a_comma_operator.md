## [What is the advantage of a comma operator](#what-is-the-advantage-of-a-comma-operator)

### What is the advantage of a comma operator?

The comma operator allows you to evaluate multiple expressions and return the result of the last one, all within a single statement. This can help in certain cases where you want to write concise code, especially in loops or complex expressions.

Example:

```javascript
let x = (a = 1, b = 2, a + b);
console.log(x); // 3
```

**Tags**: basic, JavaScript, operators


