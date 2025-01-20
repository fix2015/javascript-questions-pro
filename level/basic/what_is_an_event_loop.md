## [What is an event loop](#what-is-an-event-loop)

### What is an event loop?

The event loop is a fundamental concept in JavaScript's concurrency model. It is responsible for executing code, handling events, and executing queued messages (tasks). The event loop continuously checks the call stack and event queue, ensuring that asynchronous tasks are executed when the call stack is empty.

Example:

```javascript
console.log('Start');
setTimeout(() => console.log('Timeout'), 0);
console.log('End');
// Output: 'Start', 'End', 'Timeout'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [concurrency model](./theme/concurrency_model)


