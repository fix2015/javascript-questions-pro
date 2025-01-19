## [What are the examples of built-in higher order functions?](#what-are-the-examples-of-built-in-higher-order-functions)

### What are the examples of built-in higher-order functions?

Higher-order functions are functions that can accept other functions as arguments or return functions. Examples of built-in higher-order functions in JavaScript include:

1. **`map`**:
   ```javascript
   const numbers = [1, 2, 3];
   const doubled = numbers.map(num => num * 2);
   console.log(doubled); // [2, 4, 6]
   ```

2. **`filter`**:
   ```javascript
   const numbers = [1, 2, 3, 4];
   const evens = numbers.filter(num => num % 2 === 0);
   console.log(evens); // [2, 4]
   ```

3. **`reduce`**:
   ```javascript
   const numbers = [1, 2, 3, 4];
   const sum = numbers.reduce((total, num) => total + num, 0);
   console.log(sum); // 10
   ```

4. **`forEach`**:
   ```javascript
   const numbers = [1, 2, 3];
   numbers.forEach(num => console.log(num));
   ```

5. **`sort`**:
   ```javascript
   const names = ['Charlie', 'Alice', 'Bob'];
   names.sort((a, b) => a.localeCompare(b));
   console.log(names); // ['Alice', 'Bob', 'Charlie']
   ```

**Tags**: basic, JavaScript, Functional Programming


