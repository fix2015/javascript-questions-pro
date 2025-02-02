## [How do you implement a Queue in JavaScript?](#how-to-implement-a-queue-in-javascript)

### How do you implement a Queue in JavaScript?

A queue can be implemented using an array or linked list. For simplicity, let's use an array.

Example of a queue implementation using an array:

```javascript
class Queue {
  constructor() {
    this.items = [];
  }
  enqueue(element) {
    this.items.push(element);
  }
  dequeue() {
    return this.items.shift();
  }
  peek() {
    return this.items[0];
  }
  isEmpty() {
    return this.items.length === 0;
  }
}
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Implementation](./theme/implementation)


