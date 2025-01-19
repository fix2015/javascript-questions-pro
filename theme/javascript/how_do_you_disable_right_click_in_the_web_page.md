## [How do you disable right click in the web page](#how-do-you-disable-right-click-in-the-web-page)

### How do you disable right click in the web page?

You can disable right-click by listening for the `contextmenu` event and preventing its default behavior.

Example:

```javascript
document.addEventListener('contextmenu', function(event) {
  event.preventDefault();
  console.log('Right-click is disabled');
});
```

**Tags**: intermediate, JavaScript, DOM


