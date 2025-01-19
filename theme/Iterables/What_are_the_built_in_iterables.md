## [What are the built-in iterables](#what-are-the-built-in-iterables)

### What are the built-in iterables?

Built-in iterables in JavaScript include:

1. **Arrays**:
   ```javascript
   for (let item of [1, 2, 3]) {
     console.log(item);
   }
   ```

2. **Strings**:
   ```javascript
   for (let char of 'hello') {
     console.log(char);
   }
   ```

3. **Maps** and **Sets**:
   ```javascript
   let map = new Map([['a', 1]]);
   for (let [key, value] of map) {
     console.log(key, value);
   }
   ```

4. **Typed Arrays** and **NodeLists**.

**Tags**: intermediate, JavaScript, Iterables


