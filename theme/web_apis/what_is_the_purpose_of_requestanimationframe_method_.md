## [What is the purpose of requestAnimationFrame method?](#what-is-the-purpose-of-requestanimationframe-method)

### What is the purpose of `requestAnimationFrame` method?

`requestAnimationFrame` is used to schedule animations in the browser for optimal performance.

#### Key Points:
1. **Synchronizes with Refresh Rate:**
   - Ensures smooth animations by aligning with the screen refresh rate.

2. **Efficient Rendering:**
   - Avoids unnecessary frame rendering when the tab is inactive.

Example:
```javascript
function animate() {
  // Animation logic here
  console.log('Animating...');
  requestAnimationFrame(animate);
}

requestAnimationFrame(animate);
```

**Tags**: intermediate, JavaScript, Web APIs


