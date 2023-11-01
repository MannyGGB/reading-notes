# Reading 09

(https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

- What is functional programming? It is a way of building computer programmes using the evaluation of mathematical functions and avoiding changing state or data that can change.
- What is a pure function and how do we know if something is a pure function? Pure functions are used to structure functional programming and have two characteristics: the result returned should always be the same if given the same arguments, and the function does not have any side effects.
- What are the benefits of a pure function? The code is easier to test and you don't need any mock tests. The code is more reliable and easy to read and refactor too.
- What is immutability? When data is immutable, it cannot change after its creation. To change it, you have to create a new object with the new value.
- What is Referential transparency? It is when a pure function uses immutable data, consistently returning the same value for the same input.

(https://www.youtube.com/watch?v=xHLd36QoS4k)

- What is a module? A module is a part of the code with one functionality. We can call those modules whenever we need them. Separating the different fucntionalities into modules helps with structuring and readability, being on different files. In theory, it sounds very similar to components in React.
- What does the word ‘require’ do? The require function is used to call upon another module and use its functionality elsewhere, usually in the main app file. The require function passes a string with the file location in it ("./count").
- How do we bring another module into the file the we are working in? We need to export the module element we want to use (module.exports = counter).
- What do we have to do to make a module available? We need to declare a variable for the require function with the same name as the variable exported. For example, if we exported "counter," the variable for the require function should be "counter" too.
