# Class 04 (26/10/2023)

## Morning Challenge

- What is React? A user interface library.
- What is JSX? JS and HTML combined in a language.
- What is a component in React? An independent and reusable piece of code encapsulating a function.
- How do you create a functional component in React? By creating a JS function.
- How do you manage the state in a component? With useState().
- How do you add comments in JSX? ctrl + / or {/\* \*/}
- What is the purpose of the useState hook? useState is a hook that allows you to have state variables in functional components. You pass the initial state to this function, and it returns a variable with the current state value (not necessarily the initial state) and another function to update this value.
- What is a hook in React? Hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don't work inside classes — they let you use React without classes.
- What is React's Virtual DOM? The virtual DOM (VDOM) is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM. This process is called reconciliation.

## React and Forms

<form onSubmit={function} /> this is how we handle the form submit
<input onChange={}/> tracks the input and does something when it happens (we can decide what to do with an event function)
(...)spread --> we use spread to take the properties of an object or items in an array to move them into a new object or array. We can add new properties or items to the new object or array too.
