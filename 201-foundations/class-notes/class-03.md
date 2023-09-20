# Class 03 (20/09/2023)

## HTML

span --> adds a section in the website with no inherent value. Adds a space to be filled.

## CSS the Box Model

Content < Padding < Border < Margin
background is included in the padding
margin: 10px 20px; first number is top and bottom / second number is left and right

## For loops and arrays / While loops (many times) and if (one time)

## JS arrays

// Arrays
// Arrays are lists of data
// comma delimited
// zero indexed
let team = ["Tim", "Rich", "Sam", "Jez"]; // .length is 3 in this case
console.log("Hello " + team[0]) // 0 is the first item
// we can store anything in an array (string, number, object, array)
// initialisation; condition; increment
for(let i = 0; i < team.length; i++){
console.log("Hello " + team[i]) // by writing the i variable, you can keep adding items to the array, as the i variable is incrementing
}

let arr = [];

let foodItem = prompt("What food do you like?")
arr.push(foodItem) // push adds the input at the end of the array
arr.pop() // removes the last item
arr.unshift() // adds an item to the beginning of the array
arr.shift() // removes the first item
arr.indexOf() // to tell the position of an item in an array. -1 means is not in the array
arr.splice(index, deleteCount, itemToAdd--optional) // adds or removes item at a specific location
console.log(arr)

## Operators

// Evaluating Comparisons
// syntax
operand operator operand
1 < 2 // evaluates true
1 === 2 // evaluates false
1 === 1 // evaluates true

// === strictly equal to
// !== not equal to
// <= less than or equal
// < less than
// >= greater than or equal to
// > greater than

// && AND
// || OR

1 < 2 && 3 < 4 // true
true && true

"Tim" === "tim" || "rich" !== "Rich" // true
false || true

// truthy , falsy
//falsy
false
0
""
let a; // undefined
null
"5" / 2 // NaN Not a Number

## Lab Hint

let userPoints = 0
// we are making sure the user writes the name input
let userName = prompt("Tell me your name")
while(!userName) {
userName = prompt("You need to tell me.")
}
// a question with multiple answers
let favFoods = ["pizza", "pasta", "garlic bread"]

let foodAns = prompt("What is one of Tim's fav foods?").toLowerCase();

for(let i = 0; i < favFoods.length; i++) {
if (foodAns === favFoods[i]) {
alert("Nice")
userPoints++;
}
alert("you got" + userPoints + out of correct)
}

if(favFoods.indexOf(foodAns))

## Review

<a href="mailto: email@email.com"> --> send an email to that address

header, footer{ --> this targets both header and footer
background-color: red
}

trim() --> removes the trailing spaces after an answer

let ans = "yes"

ans === "yes" // true
ans === "no" // false
ans !== "yes" // false
ans !== "no" // true

// make sure it is yes or no in the input
while(ans !== "yes" && ans !== "no"){
ans = prompt("Answer yes or no").toLowerCase;
}

let ans1 = prompt("Pick a number.")

// runs 1 time
if (ans1 !== "7"){
ans = prompt(Wrong number)
}
// runs until () becomes false
while (ans1 !== "7"){
ans = prompt(Wrong number)
}
true && false // falsey
false || true // truthy
false && true // falsey
true || false // truthy

&& needs both sides to be true
|| only needs one side to be true

let myCities = [
"Granada",
"Cordoba",
"Toledo",
"Barcelona",
"Santiago de Compostela",
"Valencia",
"Salamanca",
"Palma de Mallorca",
"Santander",
"Bilbao",
];
let myCitiesAnswer = prompt(
"Name one of my top 10 Spanish cities."
).toLowerCase();
for (let i = 1; i < 6; i++) {
for (let i2 = 0; i2 < myCities.length; i2++) {
if (myCitiesAnswer === myCities[i2]) {
alert("Well done! You can visit on your next holiday!");
break;
userPoints++;
} else {
myCitiesAnswer = prompt("Try again!");
}
if (i == 5) {
i = alert("Sorry, the answers are " + myCities + ".");
}
}
}
