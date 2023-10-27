# Reading 05

(https://react.dev/learn/thinking-in-react)

- What is the single responsibility principle and how does it apply to components?
  Each componenet should only have one action to do, one responsibility. If a component is doing more than one action, maybe it should be split into other componenents. For example, you could have a component to keep your state separate from a component displaying a form.
- What does it mean to build a ‘static’ version of your application? Build the main components without any functionality (state) to make source all components are nested correctly and props are passed down from parent to children.
- Once you have a static application, what do you need to add? You can add state and build the functions around the components you have.
- What are the three questions you can ask to determine if something is state?
  1. "Does it remain unchanged over time? If so, it isn’t state.
  2. Is it passed in from a parent via props? If so, it isn’t state.
  3. Can you compute it based on existing state or props in your component? If so, it definitely isn’t state!"
- How can you identify where state needs to live? You can follow these steps:
  "Often, you can put the state directly into their common parent.
  You can also put the state into some component above their common parent.
  If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component."

(https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

- What is a “higher-order function”? It is a function that works on another function; for example, we can have a function that creates another function or a function that changes another function.
- Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
  This function returns a function with a parameter (m) and a condition (if m is more than n, n being the parameter of the higher-order function). As we can see, the parameter n equals 10 and the parameter m equals 11, so the condition is true.
- Explain how either map or reduce operates, with regards to higher-order functions.
  The map method goes through and array and returns a new array that can be changed without changing the original array we are mapping. We can use map to go through an array and then use a function to add new values or change the previous values in the new array.
  The reduce method goes through an array and combines the array item with another value, returning a new value. It usually takes three parameters: the array, the combining function, and the start value. We can use a function to set up the reduce method and then another to combine the value and the index value. For example:

```
reduce([1, 2, 3, 4], (a, b) => a + b, 0) //reduce([array], combining arrow function, start value)
//This returns 10 (I think it goes 0 + 1 = 1, 1 + 2 = 3, 3 + 3 = 6, 6 + 4 = 10).

```
