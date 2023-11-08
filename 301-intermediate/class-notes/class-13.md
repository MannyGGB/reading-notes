# Class 13 (08/11/2023)

## Morning Challenge

<!--  CSS challenge -->

div {
display: flex;
justify-content: center;
margin: 200px;
}

.slit-in-vertical {
background-color: purple;
color: yellow;
padding: 20px;
border-radius: 5px;
font-size: 1rem;
font-family: monospace;
-webkit-animation: slit-in-vertical 0.45s ease-out both;
animation: slit-in-vertical 0.45s ease-out both;
}

@-webkit-keyframes slit-in-vertical {
0% {
-webkit-transform: translateZ(-800px) rotateY(90deg);
transform: translateZ(-800px) rotateY(90deg);
opacity: 0;
}

54% {
-webkit-transform: translateZ(-160px) rotateY(87deg);
transform: translateZ(-160px) rotateY(87deg);
opacity: 1;
}

100% {
-webkit-transform: translateZ(0) rotateY(0);
transform: translateZ(0) rotateY(0);
}
}

@keyframes slit-in-vertical {
0% {
-webkit-transform: translateZ(-800px) rotateY(90deg);
transform: translateZ(-800px) rotateY(90deg);
opacity: 0;
}

54% {
-webkit-transform: translateZ(-160px) rotateY(87deg);
transform: translateZ(-160px) rotateY(87deg);
opacity: 1;
}

100% {
-webkit-transform: translateZ(0) rotateY(0);
transform: translateZ(0) rotateY(0);
}
}

## Lab review

- For booleans, we need to set the value to **false** to start with in the object template.
- To use checkboxes with onChange, we need to add a condition with event.target.type === "checkbox", so when we tick the box, it targets it, and [event.target.name]: event.target.value, so it adds the input.

## Update (PUT)

- Use app.put to create a new endpoint with params /:id.
- findByIdAndUpdate()
- When updating the form, make sure that in input, the name and value match.
- Optional chaining --> movie?.name (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining)
- Nullish coalescing --> movie ?? {object}(https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Nullish_coalescing)
