## [How do you create polyfills for map, filter and reduce methods?](#how-do-you-create-polyfills-for-map-filter-and-reduce-methods)

### How do you create polyfills for `map`, `filter`, and `reduce` methods?

#### `map` Polyfill:
```javascript
Array.prototype.myMap = function(callback) {
  const result = [];
  for (let i = 0; i < this.length; i++) {
    if (this.hasOwnProperty(i)) {
      result.push(callback(this[i], i, this));
    }
  }
  return result;
};
```

#### `filter` Polyfill:
```javascript
Array.prototype.myFilter = function(callback) {
  const result = [];
  for (let i = 0; i < this.length; i++) {
    if (this.hasOwnProperty(i) && callback(this[i], i, this)) {
      result.push(this[i]);
    }
  }
  return result;
};
```

#### `reduce` Polyfill:
```javascript
Array.prototype.myReduce = function(callback, initialValue) {
  let accumulator = initialValue;
  for (let i = 0; i < this.length; i++) {
    if (this.hasOwnProperty(i)) {
      accumulator = callback(accumulator, this[i], i, this);
    }
  }
  return accumulator;
};
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Polyfills](./theme/polyfills)


