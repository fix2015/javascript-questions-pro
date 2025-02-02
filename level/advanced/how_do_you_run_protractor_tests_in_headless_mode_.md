## [How do you run Protractor tests in headless mode?](#how-to-run-protractor-tests-in-headless-mode)

### How do you run Protractor tests in headless mode?

To run Protractor tests in headless mode, you can configure the `protractor.conf.js` file to use a headless browser like Chrome.

Example configuration:

```javascript
capabilities: {
  'browserName': 'chrome',
  'chromeOptions': {
    args: ['--headless', '--disable-gpu', '--window-size=800x600']
  }
},
```

**Tags**: [advanced](./level/advanced), [Protractor](./theme/protractor), [Headless Testing](./theme/headless_testing)


