## [How do you implement a Priority Queue in JavaScript?](#how-to-implement-a-priority-queue-in-javascript)

### How do you implement a Priority Queue in JavaScript?

A priority queue is a special type of queue where each element is assigned a priority. The element with the highest priority is dequeued first.

Example implementation using an array:

```javascript
class PriorityQueue {
  constructor() {
    this.items = [];
  }
  enqueue(element, priority) {
    const queueElement = { element, priority };
    let added = false;
    for (let i = 0; i < this.items.length; i++) {
      if (queueElement.priority < this.items[i].priority) {
        this.items.splice(i, 0, queueElement);
        added = true;
        break;
      }
    }
    if (!added) {
      this.items.push(queueElement);
    }
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

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Data Structures](./theme/data_structures)


