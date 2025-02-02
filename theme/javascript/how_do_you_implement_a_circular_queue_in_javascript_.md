## [How do you implement a Circular Queue in JavaScript?](#how-to-implement-circular-queue-in-javascript)

### How do you implement a Circular Queue in JavaScript?

A circular queue implementation requires maintaining two pointers (front and rear) and using modulo arithmetic to handle wraparound.

Example:

```javascript
class CircularQueue {
  constructor(size) {
    this.size = size;
    this.queue = new Array(size);
    this.front = 0;
    this.rear = 0;
  }
  enqueue(element) {
    if ((this.rear + 1) % this.size === this.front) {
      console.log('Queue is full');
    } else {
      this.queue[this.rear] = element;
      this.rear = (this.rear + 1) % this.size;
    }
  }
  dequeue() {
    if (this.front === this.rear) {
      console.log('Queue is empty');
    } else {
      this.front = (this.front + 1) % this.size;
    }
  }
  peek() {
    return this.queue[this.front];
  }
  isEmpty() {
    return this.front === this.rear;
  }
}
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Data Structures](./theme/data_structures)


