# Reading 10

(https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

- What is a ‘call’? A call is a function invocation. After a function is declared, you can call it at any point in your code.
- How many ‘calls’ can happen at once? Calls happen one at a time from top to bottom.
- What does LIFO mean? Last In, First Out. "It means that the last function that gets pushed into the stack is the first to be pop out, when the function returns."
- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```

function one(){
 console.log("Hello from one");
}

function two(){
 one();
 console.log("The end from two");
}

two();

```

In this example, two is called first, then one is called and executed, then two is executed.

- What causes a Stack Overflow? When a function calls itself without an exit point. It continues to call itself infinitely until the browser or host reaches the maximum limit of calls.

(https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

- What is a ‘reference error’? An error appears when you try to use an element which has not been declared yet, for example, a variable. There is not previous reference to that element.
- What is a ‘syntax error’? Syntax errors are related to the incorrect structure of elements. For example, using {} for the elements of an array or ; to separate the properties in an object.
- What is a ‘range error’? Errors related to the length of elements, for example in arrays.
- What is a ‘type error’? This error shows when you are trying to access two types that are incompatible. For example, using dot notation to access a property in an object, and thos property has not been given a value yet.
- What is a breakpoint? It is a point in your code where you want to stop to check if there is an error.
- What does the word ‘debugger’ do in your code? You can add a debugger statement in your code to create a breakpoint. A common one is the use of console.log().
