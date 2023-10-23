# Class 01 (23/10/2023)

## Arrow Functions

// normal declaration
function sum(a, b) {
return a + b;
}
console.log(sum(400, 20));

// arrow function
const multiply = (a, b) => {
return a \* b;
}
console.log(multiply(21, 20));

//one line function (implicit return)
const substract = (a, b) => a - b;

const divideBy12 = a => a / 12;

## Classes

//constructors
function OldAnimal(name, colour, age) {
this.name = name;
this.colour = colour;
this.age = age;
}
OldAnimal.prototype.speak = function() {console.log(this.name + " shouts")};

// classes
class Animal {
constructor(name, colour, age) {
this.name = name;
this.colour = colour;
this.age = age;
}
speak = () => {
console.log(`${this.name} makes a noise`);
}
}

class Dog extends Animal {
constructor(name, colour, age, breed) {
super (name, colour, age);
this.breed = breed;
}
goodBoi = () => {
console.log(`You pat ${this.name} on the head.`);
}
}

const spot = new Dog ("Spot", "yellow", 43, "Pointer");
console.log(spot)
spot.speak()
spot.goodBoi()

## React and Vite

- Create a project in React with Vite:

1. npm create vite@latest
2. Give it a name, Pick React, Pick Javascript
3. cd my-project
4. npm install
5. git init
6. npm run dev

GitHub

1. Create an empty repository (do NOT add a README.md file)
2. Follow the 'push an existing repository from your computer 'instructions on github
3. You may need to go git add . and git commit -m 'message' before you can push.

.env added to the .gitignore
