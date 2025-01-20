## [What is a microtask queue](#what-is-a-microtask-queue)

### What is a microtask queue?

A microtask queue is a queue in JavaScript that handles microtasks, which are small asynchronous tasks. These tasks are executed after the current script finishes executing, but before any other tasks in the event loop (macrotasks) are processed.

Microtasks typically include promise handlers (`.then()`, `.catch()`) and tasks queued by `queueMicrotask()`.

Example:

```javascript
Promise.resolve().then(() => console.log('Microtask executed'));

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Event Loop](./theme/event_loop)


