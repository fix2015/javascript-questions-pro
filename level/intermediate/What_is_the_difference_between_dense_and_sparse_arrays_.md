## [What is the difference between dense and sparse arrays?](#what-is-the-difference-between-dense-and-sparse-arrays)

### What is the difference between dense and sparse arrays?

- **Dense Arrays**:
  - All indices have elements assigned.
  - Example:
    ```javascript
    const denseArray = [1, 2, 3];
    console.log(denseArray.length); // 3
    ```

- **Sparse Arrays**:
  - Some indices are missing (unassigned).
  - Example:
    ```javascript
    const sparseArray = [1, , 3];
    console.log(sparseArray.length); // 3
    console.log(sparseArray[1]); // undefined
    ```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays)


