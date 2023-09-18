# Class 07 (14/09/2023)

- Review (HTML5, CSS, JavaScript)
- JS Functions

- Vocabulary
    - Script
    - Programatic Problem Solving --> look at problems, solve them step by step
    - Expression
    - Operator
    - Function
        - Declaration {}
        - Call --> invoke
        - Parameters
        - Arguments
        - Return value
    - Refactoring --> optimise code, make it more efficient, keeping the same functionality

- Give instructions to robot to watch Rick Astley's Never Gonna Give You Up on YouTube.
    1. Click on the search bar
    2. Type *YouTube.com*
    3. Press *Enter*
    4. Click on the search bar
    5. Type *Rick Astley's Never Gonna Give You Up*
    6. Press *Enter*
    **Instructions need to be very literal to get a specific result**

## Operators
+ - * / etc
## Expressions --> when we compare two things and evaluates a value
let a = 1 + 2
let b = 1 * 2
let c = 2 - 1
let d = 1 / 2
let e = 1 ** 2

## Comparators
== equal to
!= not equal to
>
<
>=
<=
=== strictly equal to
!== strictly not equal to

## Comparisons
a > b --> false (false is the value after being evaluated)
c <= d
d >= c

## Parameters
They are inside the function brackets
function sum(num1, num2) {
    console.log(num1 + num2)
}

let a = prompt("Give me num1")
let b = prompt("Give me num2")

sum(a, b)

