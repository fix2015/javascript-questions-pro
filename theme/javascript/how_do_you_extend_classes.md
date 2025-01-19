## [How do you extend classes](#how-do-you-extend-classes)

### How do you extend classes?

In JavaScript, you can extend a class using the `extends` keyword. This allows a subclass to inherit properties and methods from a parent class.

Example:

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
  speak() {
    console.log(`${this.name} makes a sound`);
  }
}
class Dog extends Animal {
  speak() {
    console.log(`${this.name} barks`);
  }
}
const dog = new Dog('Buddy');
dog.speak(); // 'Buddy barks'
```

**Tags**: intermediate, JavaScript, classes


