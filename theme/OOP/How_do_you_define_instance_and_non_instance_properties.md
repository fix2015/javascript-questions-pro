## [How do you define instance and non-instance properties](#how-do-you-define-instance-and-non-instance-properties)

### How do you define instance and non-instance properties?

- **Instance Properties**:
  - Defined within the constructor using `this`.
  - Specific to each instance of a class.

- **Non-Instance Properties**:
  - Defined on the class itself (static properties).
  - Shared across all instances.

Example:

```javascript
class Example {
  constructor(name) {
    this.name = name; // Instance property
  }
  static type = 'Example'; // Non-instance property
}
console.log(Example.type); // Output: 'Example'
```

**Tags**: intermediate, JavaScript, OOP


