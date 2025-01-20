## [What is the difference between reflow and repaint](#what-is-the-difference-between-reflow-and-repaint)

### What is the difference between reflow and repaint?

Reflow is the process where the browser recalculates the layout of the page, whereas repaint only redraws elements that have changed visually, without affecting the layout.

Example:

```javascript
// Reflow happens when you modify layout-affecting properties like width/height
document.body.style.width = '500px';  // Triggers reflow

// Repaint happens when you modify visual properties like background-color
document.body.style.backgroundColor = 'red';  // Triggers repaint
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Performance](./theme/performance)


