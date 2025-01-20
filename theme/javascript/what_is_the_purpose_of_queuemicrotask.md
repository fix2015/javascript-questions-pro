## [What is the purpose of queueMicrotask](#what-is-the-purpose-of-queuemicrotask)

### What is the purpose of `queueMicrotask`?

The `queueMicrotask()` method is used to add a microtask to the event loop queue. It is similar to using a promise but ensures that the task will be executed as soon as the current task completes, before any rendering or other tasks.

Example:

```javascript
queueMicrotask(() => console.log('Microtask executed'));

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Event Loop](./theme/event_loop)


