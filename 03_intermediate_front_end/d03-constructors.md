## Constructors

#### Description

Constructors are blueprints to create objects. We define a function that accepts arguments. We then create a new **instance** of an object (through **instantiation**).

#### In-Class Examples

```javascript
// the giver (todo: read)

function Person(name, age, fact) {

  // assign properties to an object
  this.name = name;
  this.age = parseInt(age);
  this.fact = fact;

}



// bike constructor
// it creates an object
// a constructor is a blueprint to construct an object
// speeds, colour, size, price, brand
function Bike(speeds, colour, size, price, brand) {

  // attributes
  this.speeds = speeds;
  this.colour = colour;
  this.size = size;
  this.price = price;
  this.brand = brand;

  // abilities
  this.toString = function() {
    return 'This bike has ' + this.speeds + ' and is ' + this.colour;
  }

}
// declare a variable called annasBike
// create a 'new' INSTANCE of 'Bike'
// create a new copy of bike
var annasBike = new Bike(21, 'teal', 'small', 350, 'diamondback');
annasBike.toString();
var jamesBike = new Bike(6, 'white', 'medium', 200, 'biria');
jamesBike.toString();
```


### The this keyword references each individual `instance` of an object,
### that means everytime we call `new Bike()` we are creating a new object
### and our this is referencing that unique object everytime. 
