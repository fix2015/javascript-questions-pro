## [What are the different kinds of generators](#what-are-the-different-kinds-of-generators)

### What are the different kinds of generators?

Generators can be categorized based on their usage:

1. **Simple Generators**: Yield a series of values.
   ```javascript
   function* simpleGenerator() {
     yield 1;
     yield 2;
     yield 3;
   }
   ```

2. **Delegating Generators**: Use `yield*` to delegate to another generator or iterable.
   ```javascript
   function* delegatingGenerator() {
     yield* [1, 2, 3];
   }
   ```

3. **Asynchronous Generators**: Use `async` and `for await...of` for asynchronous operations.
   ```javascript
   async function* asyncGenerator() {
     yield await Promise.resolve(1);
   }
   ```

**Tags**: advanced, JavaScript, Generators


