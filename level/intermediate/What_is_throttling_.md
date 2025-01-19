## [What is throttling?](#what-is-throttling)

### What is throttling?

Throttling ensures that a function is called at most once in a specified time interval. It is useful for rate-limiting events like scrolling or resizing.

Example:

```javascript
function throttle(func, limit) {
  let inThrottle;
  return function(...args) {
    if (!inThrottle) {
      func.apply(this, args);
      inThrottle = true;
      setTimeout(() => (inThrottle = false), limit);
    }
  };
}

const log = throttle(() => console.log('Throttled!'), 1000);
window.addEventListener('scroll', log);
```

**Tags**: intermediate, JavaScript, Performance


