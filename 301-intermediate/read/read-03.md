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

- Give an example of using the spread operator to add a new item to an array. (https://www.samanthaming.com/tidbits/87-5-ways-to-append-item-to-array/#spread)
  const ocean = ['🐙', '🦀'];

const aquarium = [...ocean, '🐡']; // Add a single value
const sushi = [...ocean, '🐡', '🍚']; // Add multiple values

aquarium; // ['🐙', '🦀', '🐡']
sushi; // ['🐙', '🦀', '🐡', '🍚']

- Give an example of using the spread operator to combine two objects into one.
  const obj1 = { foo: "bar", x: 42 };
  const obj2 = { bar: "baz", y: 13 };

const mergedObj = { ...obj1, ...obj2 };
// { foo: "bar", x: 42, bar: "baz", y: 13 }
If we merge objects with the same properties, the value of the last object's properties stay.

(https://www.youtube.com/watch?v=c05OL7XbwXU)

- In the video, what is the first step that the developer does to pass functions between components? He declares a function in the parent component to keep the state that is going to be changed, in this case, a counter.
- In your own words, what does the increment function do? The increment function goes through an array of people using .map, and if the property name in the new array matches the property name in the old array, the property count in the new array increases by 1 and that object person goes into the new array.
- How can you pass a method from a parent component into a child component? Same as you would do with a prop. In this case, it creates a new tag for the <Person /> using this (the function is inside an object).
- How does the child component invoke a method that was passed to it from a parent component? In this case, we can use this (to refer back to the parent object where the function is) props (because the property is passed from parent to child) and the name of the function with (). this.props.increment().
