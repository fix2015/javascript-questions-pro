## [What are the differences between for...of and for...in statements](#what-are-the-differences-between-forof-and-forin-statements)

### What are the differences between for...of and for...in statements?

- **`for...of`**:
  - Iterates over values of an iterable (e.g., array, string, Map).
  - Example:
    ```javascript
    for (let value of [10, 20, 30]) {
      console.log(value); // 10, 20, 30
    }
    ```

- **`for...in`**:
  - Iterates over keys or properties of an object.
  - Example:
    ```javascript
    for (let key in { a: 1, b: 2 }) {
      console.log(key); // 'a', 'b'
    }
    ```

**Tags**: basic, JavaScript, Loops


