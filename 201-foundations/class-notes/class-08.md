# Class 08 (27/09/2023)

## Lab Review

- Focus on prototype, constructors, and HTML tables

## CSS Layouts

- CSS reset website: copy and paste the code into a CSS file to reset browser default formatting.
- display: flex; always goes on the parent, not on the individual children (for example, in section, not the divs inside the section).
- flex-direction: is set to row by default, can be changed to column.
- flex-wrap: wrap; when the items don't fit, the move to a new line instead of squeezing in.
- justify-content: flex-end/flex-start/center; aligns the content in different ways. It works on the MAIN AXIS.
- justify-content: space-around, space-between, space-evenly; adds space in different ways in between content.
- align-content: same as justify-content, but it works on the CROSS AXIS.
- align-self: for individual items.

section {
background-color: tomato;
width: 90%;
margin: 0 auto;
height: 500px;
border: 5px solid black;
display: flex;
}
justify-content: flex-end/flex-start/center;
justify-content: space-around, space-between, space-evenly;
