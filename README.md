## Quiz: Reviewing JavaScript Inheritance

???

# Reviewing JavaScript Inheritance

?: What is the native object orientation model of JavaScript?

(X) Prototypal
() Class-Based
() ES2016 standard
() Prototypical

?: The primary difference between an object created by a factory function and a constructor function is:

() Factory functions cannot create objects with methods
(X) Constructor functions’ creations identify their constructor as the constructor name
() Constructor functions cannot create instances of type Object
() Factory functions are more memory efficient

?: With a constructor function called `Dog()`, we can assume that the `typeof` its `prototype` attribute is:

() `Class`
(X) `object`
() Undefined
() Constructor

?: Given the following constructor function: 

```javascript
function Dog(name){ this.name = name}
```

Which we can assume to be assigned to `let b = new Dog(“Byron”)`.

Which code sample below would add a method called `bark()` to the prototype that returns “Byron says bark”?

()
```javascript
function Dog(name){ this.name = name; this.bark = () => console.log(`${this.name} says bark`) }
````
() 
```javascript
function Dog(name){ this.name = name; this.bark = function() { console.log(`${this.name} says bark`) } }
```
() 
```javascript
b.prototype = () => console.log(`${this.name} says bark`)
````
(X) 
```javascript
Dog.prototype.bark =  () => console.log(`${this.name} says bark`)
```

?: Given the following code, how many definitions of `razzle()` exist?

```javascript
function Wizard(name) { this.name = name }
["radegast", "gandalf", "harry potter", "merlin"].map( n => new Wizard(n.charAt(0).toUpperCase() + n.slice(1) ))
Wizard.prototype.razzle = function() {
console.log(`${this.name} razzles you!`)
}
```

() 4
(X) 1
() 0
() 5

???
