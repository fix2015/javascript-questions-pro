## [How do you test async code in Jest?](#how-to-test-async-code-in-jest)

### How do you test async code in Jest?

Jest provides `async` and `await` to test asynchronous code. You can return a promise from the test function or use `done` for callback-based code.

Example with `async`/`await`:

```javascript
test('fetches data asynchronously', async () => {
  const data = await fetchData();
  expect(data).toBeDefined();
});
```

**Tags**: [intermediate](./level/intermediate), [Jest](./theme/jest), [Async Testing](./theme/async_testing)


