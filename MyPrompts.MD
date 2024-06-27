What is a class in JavaScript?
In JavaScript, a class is a blueprint for creating objects with predefined properties and methods. It is a special syntax introduced in ECMAScript 2015 (ES6) that allows developers to implement object-oriented programming principles more conveniently.

Here’s an example of how a class is defined and used in JavaScript:

Defining a Class
class Person {
  // Constructor method for initializing new objects
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  // Method associated with the class
  greet() {
    console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
  }
}
Creating an Instance of a Class
const person1 = new Person('Alice', 30);
person1.greet(); // Output: Hello, my name is Alice and I am 30 years old.
Key Points:
Constructor: The constructor method is a special method for creating and initializing objects created with a class.
Methods: Functions defined inside a class that can operate on objects created from the class.
Instantiation: Using the new keyword to create an instance of a class.
Inheritance: Classes can extend other classes using the extends keyword, allowing for inheritance of properties and methods.
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  speak() {
    console.log(`${this.name} barks.`);
  }
}

const dog = new Dog('Rex');
dog.speak(); // Output: Rex barks.
In this example, the Dog class inherits from the Animal class, and the speak method is overridden to provide specific behavior for dogs.
