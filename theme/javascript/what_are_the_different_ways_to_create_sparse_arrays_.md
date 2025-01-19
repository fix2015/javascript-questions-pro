## [What are the different ways to create sparse arrays?](#what-are-the-different-ways-to-create-sparse-arrays)

### What are the different ways to create sparse arrays?

1. **Using Array Constructor**:
   ```javascript
   const sparseArray = new Array(3); // Creates [ <3 empty items> ]
   ```

2. **Using Comma Syntax**:
   ```javascript
   const sparseArray = [1, , 3]; // Creates [1, <1 empty item>, 3]
   ```

3. **Deleting Elements**:
   ```javascript
   const array = [1, 2, 3];
   delete array[1]; // Creates [1, <1 empty item>, 3]
   ```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Arrays](./theme/arrays)


