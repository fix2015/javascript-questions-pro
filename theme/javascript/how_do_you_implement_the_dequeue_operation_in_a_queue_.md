## [How do you implement the dequeue operation in a Queue?](#how-to-implement-dequeue-operation-in-queue)

### How do you implement the dequeue operation in a Queue?

The dequeue operation removes an element from the front of the queue. In JavaScript, you can use the `shift()` method on an array to achieve this.

Example:

```javascript
let queue = [1, 2, 3];
let dequeued = queue.shift();
console.log(dequeued);  // 1
console.log(queue);     // [2, 3]
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Operations](./theme/operations)


