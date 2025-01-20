## [What is the difference between substring and substr methods?](#what-is-the-difference-between-substring-and-substr-methods)

### What is the difference between `substring` and `substr` methods?

1. **`substring(start, end)`:**
   - Extracts characters between `start` and `end` (exclusive).

2. **`substr(start, length)`:**
   - Extracts characters starting at `start` and spanning `length` characters.

Example:
```javascript
const str = 'JavaScript';

console.log(str.substring(0, 4)); // 'Java'
console.log(str.substr(0, 4));    // 'Java'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [String Methods](./theme/string_methods)


