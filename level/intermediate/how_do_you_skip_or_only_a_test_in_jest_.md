## [How do you skip or only a test in Jest?](#how-do-you-skip-or-only-a-test-in-jest)

### How do you skip or only a test in Jest?

In Jest, you can use `.skip` to skip a test and `.only` to run a specific test.

Example:

```javascript
test.skip('this test will be skipped', () => {
  // test code
});

test.only('this test will run exclusively', () => {
  // test code
});
```

**Tags**: [intermediate](./level/intermediate), [Jest](./theme/jest), [Test management](./theme/test_management)


