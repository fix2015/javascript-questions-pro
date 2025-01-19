## [What is an event queue](#what-is-an-event-queue)

### What is an event queue?

The event queue (or message queue) is a data structure that holds tasks (or events) that are waiting to be processed. When the call stack is empty, the event loop pushes the first task from the event queue onto the stack for execution.

Example:

```javascript
setTimeout(() => console.log('Event'), 0);
console.log('Start');
// Output: 'Start', 'Event'
```

**Tags**: basic, JavaScript, concurrency model


