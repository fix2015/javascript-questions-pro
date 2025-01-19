## [What are the list of validity properties](#what-are-the-list-of-validity-properties)

### What are the list of validity properties?

Here is a list of validity properties that you can access through the `validity` property of an input element:

- **valueMissing**: If the field is required but not filled in.
- **typeMismatch**: If the input value does not match the expected type.
- **patternMismatch**: If the value doesn't match the regular expression pattern defined.
- **tooLong**: If the value exceeds the `maxlength` constraint.
- **tooShort**: If the value is too short according to the `minlength` constraint.
- **rangeUnderflow**: If the value is less than the `min` attribute.
- **rangeOverflow**: If the value is greater than the `max` attribute.
- **stepMismatch**: If the value does not meet the step constraint.
- **badInput**: If the input value is not valid for the input type.
- **customError**: If a custom validation error has been set using `setCustomValidity`.

**Tags**: intermediate, JavaScript, DOM, validation


