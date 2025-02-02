## [How do you verify UI elements in Protractor?](#how-do-you-verify-ui-elements-in-protractor)

### How do you verify UI elements in Protractor?

In Protractor, you can verify UI elements using `expect()` assertions, such as verifying text, attributes, visibility, and presence of elements.

Example:

```javascript
let heading = element(by.tagName('h1'));
expect(heading.getText()).toEqual('Welcome to Protractor');
```

**Tags**: [intermediate](./level/intermediate), [Protractor](./theme/protractor), [Verification](./theme/verification)


