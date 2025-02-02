## [How do you handle waiting in Protractor?](#how-to-handle-waiting-in-protractor)

### How do you handle waiting in Protractor?

In Protractor, you can handle waiting using `browser.wait()` and `ExpectedConditions`. This helps wait for elements to appear, disappear, or change state before interacting with them.

Example:

```javascript
let EC = protractor.ExpectedConditions;
browser.wait(EC.visibilityOf(element(by.id('submit-button'))), 5000);
```

**Tags**: [intermediate](./level/intermediate), [Protractor](./theme/protractor), [Waiting](./theme/waiting)


