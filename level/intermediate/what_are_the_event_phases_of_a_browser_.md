## [What are the event phases of a browser?](#what-are-the-event-phases-of-a-browser)

### What are the event phases of a browser?

There are three main phases of event propagation in the browser:

1. **Capturing Phase (Capture):**
   - Event travels from the root to the target element.

2. **Target Phase:**
   - Event reaches the target element.

3. **Bubbling Phase (Bubble):**
   - Event propagates back from the target to the root.

Example:
```javascript
document.getElementById('myDiv').addEventListener('click', event => {
  console.log('Capturing Phase');
}, true);

document.getElementById('myDiv').addEventListener('click', event => {
  console.log('Bubbling Phase');
});
```

**Tags**: intermediate, JavaScript, Events


