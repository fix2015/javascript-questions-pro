## [How do you call the constructor of a parent class](#how-do-you-call-the-constructor-of-a-parent-class)

### How do you call the constructor of a parent class?

In JavaScript, you can call the constructor of a parent class using the `super()` keyword inside the child class’s constructor. This allows the child class to inherit properties and methods from the parent class.

Example:

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
}
class Dog extends Animal {
  constructor(name, breed) {
    super(name); // Calls the parent constructor
    this.breed = breed;
  }
}
const dog = new Dog('Rex', 'German Shepherd');
console.log(dog.name); // Rex
```

**Tags**: basic, JavaScript, classes


