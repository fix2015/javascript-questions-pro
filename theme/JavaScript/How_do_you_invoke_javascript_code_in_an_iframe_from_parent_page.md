## [How do you invoke javascript code in an iframe from parent page](#how-do-you-invoke-javascript-code-in-an-iframe-from-parent-page)

### How do you invoke JavaScript code in an iframe from parent page?

To invoke JavaScript code inside an iframe from the parent page, you can access the iframe's `contentWindow` property, which provides a reference to the iframe's `window` object.

Example:

```javascript
const iframe = document.getElementById('myIframe');
const iframeWindow = iframe.contentWindow;
iframeWindow.someFunction(); // Calls a function in the iframe
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [iframe](./theme/iframe)


