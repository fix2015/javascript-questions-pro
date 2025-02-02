## [How do you handle alerts in Protractor?](#how-to-handle-alerts-in-protractor)

### How do you handle alerts in Protractor?

Protractor provides methods to handle JavaScript alerts, confirms, and prompts. You can use `browser.switchTo().alert()` to switch to the alert and perform actions like accepting or dismissing it.

Example:

```javascript
let alert = browser.switchTo().alert();
alert.accept();
```

**Tags**: [intermediate](./level/intermediate), [Protractor](./theme/protractor), [Alerts](./theme/alerts)


