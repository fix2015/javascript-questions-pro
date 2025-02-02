## [How do you write a simple Jest test?](#how-to-write-a-simple-jest-test)

### How do you write a simple Jest test?

To write a simple Jest test, use the `test` function, which accepts a description of the test and a callback function that contains the code to test.

Example:

```javascript
test('adds 1 + 2 to equal 3', () => {
  expect(1 + 2).toBe(3);
});
```

**Tags**: [basic](./level/basic), [Jest](./theme/jest), [Testing](./theme/testing)


