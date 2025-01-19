## [What is the difference between proto and prototype](#what-is-the-difference-between-proto-and-prototype)

### What is the difference between proto and prototype?

`proto` is an internal property (or link) to the object's prototype, while `prototype` is a property of functions (used to create new objects) that defines methods and properties shared by all instances.

Example:

```javascript
function Person(name) {
  this.name = name;
}
Person.prototype.greet = function() {
  console.log('Hello ' + this.name);
};
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


