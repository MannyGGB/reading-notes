# Catch-up 01 (16/10/2023)

- For Loops
  for (let counter = 0; counter < 5; counter++) {
  console.log("Hello")
  }

  - decreasing
    for (let i = 5; i >= 0; i--) {
    if (i === 0) {
    console.log(i, "...")
    break
    }
    console.log("hi")
    }

  - loop within loop
    for (let i = 1; i < 5; i++) {
    let row = "";
    for (let j = 1; j < 5; j++) {
    row += (i \* j) + "\t"
    }
    }

  - arrays and loop
    const numbers = [1,2,3,4,5,6,7,8,9];
    const evenNumbers = [];
    for (let i = 0; i < numbers.length; i++) {
    if (number[i] % 2 === 0) {
    evenNumbers.push(numbers[i])
    }
    }
    console.log(evenNumbers)

break --> stops the loop
continue --> skips one iteration

- While loops
  let counter = 0;
  while (counter < 5) {
  console.log("Counter is ", counter)
  counter++
  }

- Two pointers --> check two indexes in an array at the same time
