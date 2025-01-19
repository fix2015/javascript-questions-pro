## [How do you capture browser back button](#how-do-you-capture-browser-back-button)

### How do you capture browser back button?

You can capture the browser's back button by listening to the `popstate` event. This event is triggered when the active history entry changes.

Example:

```javascript
window.addEventListener('popstate', function(event) {
  console.log('Back button was pressed');
});
```

**Tags**: intermediate, JavaScript, Browser Events


