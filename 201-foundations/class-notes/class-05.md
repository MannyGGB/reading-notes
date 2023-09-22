# Class 05 (22/09/2023)

## Review

let arr = ["1", "2", "3"]
console.log(arr[0]) --> access a particular item in an array

let myInfo = ["sam", 24, "true", ["Darcy", "Charlie"]]
console.log(myInfo[3][0]) --> here we access "Darcy"

- for loop (initialisation; condition; afterthought)
  let myIndex = ["itemOne", "itemTwo", "itemThree"]
  for(let i = 0; i < myIndex.length; i++) {
  console.log(myIndex[i])
  }

- functions --> reusable blocks of code
  function myFunc (parameter1, parameter2){ --> function declaration // parameters are placeholders to be replaced by arguments when invoking the function
  return parameter1 + parameter2; --> we need to return the parameters to be used outside the function
  }
  function invokation
  myFunc (argument1, argument2) --> arguments can be changed when we reuse the function

function sum(a, b) {
let output = 0;
for (let i = 0; i < 5; i++) {
output += a + b
}
return output --> return works as a break here, it stops the loop. For the loop to run, we need to use the variable output
}
sum(10, 5)
