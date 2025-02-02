## [What are mocks in Jest?](#what-are-mocks-in-jest)

### What are mocks in Jest?

Mocks in Jest are used to simulate the behavior of real objects or functions. They are useful for isolating tests and avoiding dependencies on external systems, such as APIs or databases.

Example:

```javascript
const myFunction = jest.fn();
myFunction.mockReturnValue(10);
expect(myFunction()).toBe(10);
```

**Tags**: [intermediate](./level/intermediate), [Jest](./theme/jest), [Mocks](./theme/mocks)


