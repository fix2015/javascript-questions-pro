## [Give an example usage of rangeOverflow property](#give-an-example-usage-of-rangeoverflow-property)

### Give an example usage of rangeOverflow property

The `rangeOverflow` property checks if the value entered in an input field exceeds the maximum value specified by the `max` attribute.

Example:

```html
<input type="number" id="age" min="18" max="100">
<script>
  const input = document.getElementById('age');
  if (input.validity.rangeOverflow) {
    console.log('Value exceeds the maximum limit!');
  }
</script>
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [DOM](./theme/dom), [validation](./theme/validation)


