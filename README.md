## Quiz: Reviewing JavaScript Inheritance

???

# Reviewing JavaScript Inheritance

?: 

``` javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
  eats() {
    return `${this.name} is eating!`
  }
}
class Mammal {
  constructor(name) {
    this.name = name;
  }
  sleeps() {
    return `${this.name} is sleeping!`
  }
}
class Rabbit extends Mammal {
  //...
} 
let animal = new Animal("Ringo");
let mammal = new Mammal("Wilbur");
let rabbit = new Rabbit("Jabby");
```

Which function will not output “[Name] is sleeping!”

( ) None of the above ( ) `mammal.sleeps()` (X) `animal.sleeps()` ( ) `rabbit.sleeps()`

?: You do NOT need to use the `super` keyword when declaring the constructor in a child class:

( ) True (X) False

?: 

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
  eats() {
    return `${this.name} is eating!`
  }
}
class Rabbit extends Animal {
  constructor(name, color) {
    //..
  }
}
```

What is the correct way to have the constructor for `rabbit` inherit the `name` property?

( ) `this.name = name;` (X) `super(name);` ( ) `this.name = super(name);` ( ) `super(name) = name;`

?: What keyword does JavaScript provide for directly working with a parent class constructor and inherited methods?

(X) `super` ( ) `extends` ( ) `class` ( ) `constructor`

?: 

```javascript
class Vehicle {
  constructor( make ) {
    this._make = make
  }

  get make() {
    return this._make
  }

 static definition() {
    return 'A vehicle is used for transporting people or goods, especially on land.'
  }
}

class Car extends Vehicle {
  constructor( make , driveTrain ) {
    super( make )
    this._driveTrain = driveTrain
  }

  static definition() {
    return `${super.definition()} A car is a road vehicle, typically with four wheels, powered by an internal combustion engine and able to carry a small number of people.`
  }
}
```

What is the correct way to have the `Car` utilize the inherited static method of `definition`?

( ) `definition()` ( ) `this.definition()` ( ) `super.definition` (X) `super.definition()`

???
