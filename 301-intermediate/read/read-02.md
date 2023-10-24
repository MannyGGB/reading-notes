# Reading 02

(https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? The "render" during the render phase goes first; the "componentDidMount" goes after in the commit phase.
- What is the very first thing to happen in the lifecycle of React? The mounting phase.
- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React - Updates.
  constructor, render, componentDidMount, React - Updates, componentWillUnmount (only if/when a component is removed).
- What does componentDidMount do? "If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions."

(https://www.youtube.com/watch?v=IYvD9oBCuJI)

- What types of things can you pass in the props? Props are arguments to a function. We use props to display information such as titles, descriptions, which are not going to change inside the component; they are just passed on from parent to child.
- What is the big difference between props and state? Props are passed to a component, and are handled and updated outside the component. State is handled inside the component and you need to update it inside too.
- When do we re-render our application? We need to re-render our application when we change the state inside it. so the most recent update of that information is rendered.
- What are some examples of things that we could store in state? For example, a counter that needs updating based on user input, or the information from a form. This information is only handled inside the component, but needs updating when new information is input, so we use state for that.
