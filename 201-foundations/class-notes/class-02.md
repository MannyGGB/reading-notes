# Class 2 (19/09/2023)

## Describe

- Semantic HTML
- JS data types (string, number, boolean)
- CSS selectors, rules, properties
- Files, folders, website scaffolding

## Execute

- Create and manipulate arrays in JS
- Create and scaffold a basic HTML with semantic tags
- Link external CSS and JS in the HTML head tag
- ACP using git and GitHub

##User Stories

- To identify what the functionality and design of a product should be by considering the interests and motivations of people with varied multiple points of view.
- As a **, I want **, so that...
  - As a teacher, I want to have a database with my students' marks, so that I can input and check data easily.

### Feature Tasks

- individual tasks that must be completed by the developer to accomplish the user story. Once all of the feature tasks for an individual user story is completed, so is the story.

## JS example

    let answer1 = confirm("Are you ready to rumble?");
    if (answer1 == true) {
    console.log("Great!");
    } else if (answer1 == false) {
    console.log("Bummer!");
    }

let first = true;
let second = false;
let third = true;

if (first && third) {
console.log("First and third were both true");
} else if (first || second) {
console.log("First or second was true");
} else if (third) {
console.log("Third is true");
} else {
console.log("Is anything real?");
}

let colour = prompt("What is your favourite colour?");
// switch is a conditional to check a long list of values. Similar to else if statement
switch (
colour.toLowerCase() //toLowerCase changes the input to lowercase regardless of how it was written
) {
case "purple": //You can concatenate input before break
case "red":
console.log("Your favourite colour was red");
break;
case "blue":
console.log("Your favourite colour was blue");
break;
default: // default is similar to else
console.log("I don't know your colour.");
}
