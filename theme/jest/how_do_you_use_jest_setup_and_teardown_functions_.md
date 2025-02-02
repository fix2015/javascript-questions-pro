## [How do you use Jest setup and teardown functions?](#how-to-use-jest-setup-and-teardown-functions)

### How do you use Jest setup and teardown functions?

Jest provides two special functions: `beforeAll` and `afterAll` for global setup and teardown, and `beforeEach` and `afterEach` for setup and teardown before/after each test.

Example:

```javascript
beforeEach(() => {
  // Setup before each test
});
afterEach(() => {
  // Teardown after each test
});
```

**Tags**: [intermediate](./level/intermediate), [Jest](./theme/jest), [Setup and Teardown](./theme/setup_and_teardown)


