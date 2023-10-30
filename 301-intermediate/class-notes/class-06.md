# Class 06 (30/10/2023)

## Morning Challenge

// Write a function that takes 1 parameter (an array) and returns a new array with all the even numbers from the original array

const numbers = [9, 5, 2, -1, -10, 0, 12, 100, 289723, 2748274];

let evenNums = numbers.filter(function (arr) {
return arr % 2 === 0;
})

console.log(evenNums)
// [2, -10, 0, 12, 100, 2748274]

// The remainder % returns what's left after fitting the second value into it

3 % 2 === 1 // after putting 2 into 3, the rest is 1
4 % 2 === 0 // after putting 2 into 4, the rest is 0

# APIs (Application Programming Interface)

- APIs are used for websites to communicate with each other. It is usually a URL that returns information written in JSON.
- WRRC --> Web Request Response Cycle

  - The client requests information to the server, the server requests information to the database, the database sends a response to the server, and the server sends a response to the client.
  - Responses only come after a request.

- HTTP methods

  - POST --> create
  - GET --> read
  - PUT --> update
  - DELETE --> delete
    CRUD (create, read, update, delete)

- .env file (outside src)

  VITE_API_KEY=yourapikey
  add .env in .gitignore
  const API_KEY = import.meta.env.VITE_API_KEY
  ${API_KEY}
  On Vercel, add the content of .env to Environment Variables
