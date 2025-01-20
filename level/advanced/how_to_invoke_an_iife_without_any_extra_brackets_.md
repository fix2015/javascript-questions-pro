## [How to invoke an IIFE without any extra brackets?](#how-to-invoke-an-iife-without-any-extra-brackets)

### How to invoke an IIFE without any extra brackets?

Use an **Unary Operator** like `!` or `+` before the function to execute it immediately:

Example:

```javascript
!function() {
  console.log('IIFE invoked!');
}();

+function() {
  console.log('Another IIFE invoked!');
}();
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Functions](./theme/functions)


