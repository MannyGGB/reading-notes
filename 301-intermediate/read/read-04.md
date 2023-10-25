# Reading 04

(https://legacy.reactjs.org/docs/forms.html)

- What is a ‘Controlled Component’? It is a component whose value input is controlled by the parent component. For example, in React, the component that renders a form and also controls the input in it is a controlled component. The input value is controlled by state.
- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state - with their responses as soon as they enter them? Why? I think both options are viable, but since input is controlled by state, storing all the answers when they submit the form avoids re-rendering the page multiple times. Updating the state as soon as the user enters input, re-renders the page after every single response.
- How do we target what the user is entering if we have an event handler on an input field? We can use onChange={}

(https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

- Why would we use a ternary operator? To refactor our code into a more efficient and readable if statement. We can use ternary operators in places where if statements are not allowed. In React, you can use ternary operators in the return section, since if statements are not allowed there.
- Rewrite the following statement using a ternary statement:

```
if(x===y){
console.log(true);
} else {
console.log(false);
}

x = 1;
y = 2;
x===y ? true : false
// console.log displays false
```
