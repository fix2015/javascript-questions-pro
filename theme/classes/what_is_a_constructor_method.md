## [What is a constructor method](#what-is-a-constructor-method)

### What is a constructor method?

A constructor method in JavaScript is a special function within a class that is called when an instance of the class is created. It is used to initialize the object’s properties.

Example:

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }
}
const person = new Person('John', 30);
console.log(person.name); // John
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [classes](./theme/classes)


