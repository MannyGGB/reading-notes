# Reading 03

(https://legacy.reactjs.org/docs/lists-and-keys.html)

- What does .map() return? .map returns a new array; it doesn't change the array it uses as reference.
- If I want to loop through an array and display each value in JSX, how do I do that in React? You can use .map() and curly braces around the value/variable you want to return.
- Each list item needs a unique _key_.
- What is the purpose of a key? "Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity."

(https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

- What is the spread operator? The spread operator (...) allows you to copy all or part of an object or array into another object or array. We use it with destructuring. (paraphrased from https://www.w3schools.com/react/react_es6_spread.asp).
- List 4 things that the spread operator can do: you can copy an array or parts of an array (you can even combine it with ternary operators), you can concatenate arrays, you can copy and merge objects, you can override properties in an object (it takes the last value assigned to the saem property).
- Give an example of using the spread operator to combine two arrays.
  let arr1 = [0, 1, 2];
  const arr2 = [3, 4, 5];

  arr1 = [...arr1, ...arr2]; // this results in arr1 = [0, 1, 2, 3, 4, 5]

- Give an example of using the spread operator to add a new item to an array.

- Give an example of using the spread operator to combine two objects into one.

(https://www.youtube.com/watch?v=c05OL7XbwXU)

- In the video, what is the first step that the developer does to pass functions between components?
- In your own words, what does the increment function do?
- How can you pass a method from a parent component into a child component?
- How does the child component invoke a method that was passed to it from a parent component?
