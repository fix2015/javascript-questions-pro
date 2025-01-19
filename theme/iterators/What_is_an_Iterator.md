## [What is an Iterator](#what-is-an-iterator)

### What is an Iterator?

An iterator is an object that provides a way to access elements of a collection (such as arrays or maps) one at a time. It conforms to the `Iterator` protocol, which includes methods like `next()`, `return()`, and `throw()`.

Example:

```javascript
const arr = [1, 2, 3];
const iterator = arr[Symbol.iterator]();
console.log(iterator.next()); // { value: 1, done: false }
console.log(iterator.next()); // { value: 2, done: false }
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [iterators](./theme/iterators)


