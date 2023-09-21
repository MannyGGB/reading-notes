# Class 04 (21/09/2023)

## JS Functions

- Functions are blocks of codes that are reusable

- Function declaration
  function sayHello(){
  console.log("Hello World)
  }

- invoke (call) a function --> we can invoke functions on HTML and JS
  sayHello();

- Function parameters
  function customGreeting (user){
  console.log("Hello " + user)
  }

- invoke with parameter
  customGreeting("Manny");

- Function with multiple parameters
  function doMaths (num1, num2){
  console.log(num1 + num2);
  }

doMaths(10, 5); --> console will print 15

- Our functions return a value
  function getFullName(first, last) {
  return first + " " + last;
  }
  //when a function returns a value, we can put that value into a variable
  let fullName = getFullName ("Manny", "Gonzalez")
  console.log(fullName);

- We can put it all together
  function makePizza (promptInfo1, promptInfo2) {
  let ingredient1 = prompt(promptInfo1)
  let ingredient2 = prompt(promptInfo2)

  let output = "Here is your pizza with " + ingredient1 + ", and no " + ingredient2;
  return output
  }
  let finalPizza = makePizza("What is your fav topping?", "What is your least fav ingredient?")
  console.log(finalPizza)

## Pair Programming

- Two developers work on the same project
- Driver --> writes the code
- Navigator --> voice and thoughts. Does NOT touch the keyboard
- GitHub fork --> copy of a repository. The person who copied is now the owner of that copy, not the original owner. The original owner still has their own repository.

## CSS Layout (positioning)

We use positioning to place things wherever we want on the page.
The default positioning is static.

- top / right / bottom / left
- Position: relative -->
- Position: absolute -->
- Position: fixed -->

## Pseudo Code (break down instructions into smaller units to be coded later)

// ask the user to guess a number
// alert the user if the guess was wrong (high/low)
// ask them four times to guess
// tell them the right answer at the end, if they don't guess it

## Review

### 6th Question

let number = prompt("Guess a number between 1 and 10.");
let answer = 7;

// give the user 4 attempts at guessing (for)
for(let i = 1; i <= 4; i++){
if (parseInt(number) > answer) {
alert("Too high");
number = prompt("Guess again");
} else if (parseInt(number) < answer) {
alert("Too low");
number = prompt("Guess again");
} else if(parseInt(number) === answer) {
alert("That's right");
break;
}
} else {
alert("Not a number");
}

//give the user 4 attempts at guessing (while)
let number = prompt("Guess a number between 1 and 10.");
let answer = 7;
let attempts = 4;

while(attempts > 1) {
attempts--
if (parseInt(number) > answer) {
alert("Too high");
number = prompt("Guess again");
} else if (parseInt(number) < answer) {
alert("Too low");
number = prompt("Guess again");
} else if(parseInt(number) === answer) {
alert("That's right");
break;
}
} else {
alert("Not a number");
}
if(parseInt(number) !== answer) {
alert("The answer was 7.");
}

### 7th Questions

let answers = ["daisy", "monstera", "rich", "lilly"];
let guess = prompt("What is one of my favourite plants?");
let index = answers.indexOf(guess);

if(answers.indexOf(guess)!== -1) {
alert("Correct!")
}
