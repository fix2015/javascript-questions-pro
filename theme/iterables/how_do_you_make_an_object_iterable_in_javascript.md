## [How do you make an object iterable in JavaScript](#how-do-you-make-an-object-iterable-in-javascript)

### How do you make an object iterable in JavaScript?

To make an object iterable, you need to implement the `[Symbol.iterator]` method, which returns an iterator object.

Example:

```javascript
const iterableObject = {
  data: [1, 2, 3],
  [Symbol.iterator]() {
    let index = 0;
    let data = this.data;
    return {
      next() {
        return index < data.length
          ? { value: data[index++], done: false }
          : { done: true };
      }
    };
  }
};

for (let value of iterableObject) {
  console.log(value);  // Output: 1, 2, 3
}
```

**Tags**: advanced, JavaScript, Iterables


