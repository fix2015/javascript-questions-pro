## [What happens if you write constructor more than once in a class](#what-happens-if-you-write-constructor-more-than-once-in-a-class)

### What happens if you write constructor more than once in a class?

In JavaScript, a class can only have one constructor method. If you define multiple constructors, it will result in a syntax error. However, you can simulate multiple constructors by using default parameters or using conditional logic within a single constructor.

Example:

```javascript
class Person {
  constructor(name = 'John', age = 30) {
    this.name = name;
    this.age = age;
  }
}
const person = new Person();
console.log(person.name); // John
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [classes](./theme/classes)


