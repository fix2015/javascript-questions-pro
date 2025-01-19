## [What is microtask](#what-is-microtask)

### What is a microtask?

A microtask is a type of task that is executed after the currently executing script, but before the next task is processed. Microtasks are typically used for promises and other asynchronous operations.

Microtasks are executed after the current task completes, but before the rendering or other macrotasks are handled.

Example of a microtask:

```javascript
Promise.resolve().then(() => console.log('Microtask executed'));

**Tags**: advanced, JavaScript, Event Loop


