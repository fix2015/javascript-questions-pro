## [How do you write a simple Protractor test?](#how-to-write-a-simple-protractor-test)

### How do you write a simple Protractor test?

A simple Protractor test can be written by creating a `.spec.js` file that contains test cases using Jasmine or Mocha. You can then use `it()` to define the test case and `expect()` to assert conditions.

Example:

```javascript
describe('Example test', () => {
  it('should have a title', () => {
    browser.get('http://example.com');
    expect(browser.getTitle()).toEqual('Example Domain');
  });
});
```

**Tags**: [basic](./level/basic), [Protractor](./theme/protractor), [Testing](./theme/testing)


