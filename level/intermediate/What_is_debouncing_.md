## [What is debouncing?](#what-is-debouncing)

### What is debouncing?

Debouncing ensures that a function is called only after a specified time has passed since the last invocation. It is useful for optimizing performance in scenarios like input fields or resizing events.

Example:

```javascript
function debounce(func, delay) {
  let timer;
  return function(...args) {
    clearTimeout(timer);
    timer = setTimeout(() => func.apply(this, args), delay);
  };
}

const log = debounce(() => console.log('Debounced!'), 300);
window.addEventListener('resize', log);
```

**Tags**: intermediate, JavaScript, Performance


