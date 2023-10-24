# Class 02 (24/10/2023)

## Morning challenge

let numbers = [2, 3, 4, 5];

for (let i = 0; i < numbers.length; i++) {
console.log(numbers[i] \* numbers[i])
}

const squared = numbers.map(function(num){
return num \* num
})
console.log(squared)

## Demo recap

When we import, we can use data directly without declaring a variable.
Every function needs a return.
You can't declare variables inside the return.

## Destructuring

const {name, age} = {
name: "Sam",
age: 24
}
console.log(name, age)

By adding the properties in the const, it creates those variables and it is easier to use their values.

## .map

let array = [1, 2, 3]

let newArray = array.map(function(number) {
return number \* 2
})
console.log(newArray) --> prints [2, 4, 6]

.map is used to create a new array based on the original array.
To access specific data in the array and change it without a new array, we use .forEach.

The .map method takes two parameters max (one is the array item, which we can name, the other is the array index).

## State

import {useState} from "react"

const [likes, setLikes] = useState(0) --> likes is a variable / setLikes is a function / (0) sets the value of the variable.

function pats(){
setLikes(likes + 1) --> you can use the function and variable above in another function.
}

## State Demo (state-demo)

explorer.exe . --> opens current project in the file explorer
