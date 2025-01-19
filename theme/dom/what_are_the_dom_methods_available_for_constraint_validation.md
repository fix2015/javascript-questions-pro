## [What are the DOM methods available for constraint validation](#what-are-the-dom-methods-available-for-constraint-validation)

### What are the DOM methods available for constraint validation?

In JavaScript, constraint validation methods are used to check the validity of form inputs according to the constraints defined in the HTML form elements. The following DOM methods are available for constraint validation:

- **checkValidity()**: Checks if the element satisfies all constraints.
- **reportValidity()**: Checks validity and shows an error message if the element is invalid.
- **setCustomValidity()**: Allows you to define a custom error message for validation.

Example:

```javascript
const input = document.querySelector('input');
if (!input.checkValidity()) {
  console.log('Input is invalid');
}
```

**Tags**: intermediate, JavaScript, DOM, validation


