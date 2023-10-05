# Class 14 (05/10/2023)

## Local Storage Review

- When we setItem an object, that item is saved in local storage as a string and we cannot retrieve the information inside the object.
- If we JSON.stringify, we turn the object and properties into a string, but it loses any functions attached to the object.
- If we JSON.parse, we reinstantiate the object from a string to an object with the functions available again.

## JS Inheritance

- Prototypes are used to declare a function that can be accessed when we create new objects without having to also create the function when we create that new object.

## CSS Animation

animation-name:rotate;
animation-duration: 5s;
animation -iteration-count: infinite;

@keyframes rotate {
0%, 100% {
background: linear-gradient(-45deg, "you add the colours here");
transform: rotate(0deg)
}
50% {
background: linear-gradient(-45deg, "you add the colours here");
transform: rotate (360deg);
}
}
