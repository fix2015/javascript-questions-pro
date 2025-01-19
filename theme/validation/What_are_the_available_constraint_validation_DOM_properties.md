## [What are the available constraint validation DOM properties](#what-are-the-available-constraint-validation-dom-properties)

### What are the available constraint validation DOM properties?

The following properties are available for constraint validation in the DOM:

- **validity**: An object that contains various validity states of the input element.
- **valueMissing**: Returns `true` if the input is required but empty.
- **typeMismatch**: Returns `true` if the input value doesn't match the expected type.
- **tooLong**: Returns `true` if the value is too long for the field.
- **rangeUnderflow**: Returns `true` if the value is less than the minimum value.

Example:

```javascript
const input = document.querySelector('input');
console.log(input.validity.rangeUnderflow); // true or false
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [DOM](./theme/dom), [validation](./theme/validation)


