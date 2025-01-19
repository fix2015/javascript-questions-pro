## [What are JS labels](#what-are-js-labels)

### What are JS labels?

A label in JavaScript is used to identify a loop or a block of code, allowing you to use `break` or `continue` to exit or skip to the labeled code.

Example:

```javascript
outerLoop: for (let i = 0; i < 5; i++) {
  for (let j = 0; j < 5; j++) {
    if (i === 2 && j === 2) break outerLoop;
  }
}
```

**Tags**: basic, JavaScript, control flow

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7456494402261798177](https://www.tiktok.com/@jsmentoring/photo/7456494402261798177)
