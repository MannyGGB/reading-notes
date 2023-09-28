# Class 09 (28/09/2023)

## Wireframe Review

- It is best practice to have an \<ul\> in the \<nav\>.
- /\* is the universal selector in CSS.
- In the Inspect section, you can use a colour dropper to select a colour from the website.
- space-between adds space in between the elements, and space around also adds space at the beginning and end (this space is half of the one in between). Space-evenly adds equal space in between and at the beginning and at the end.
- margin: 0 auto --> puts element in the centre of the page.
- margin around items is 10px, and it overlaps if you put them next to each other.
- gap: creates a gap between elements.
- :hover {
  transition: 300ms; --> this changes the appearance of the button when you hover over it.
  }

## HTML Forms (with events)

<form>
  <fieldset>
    <legend>Form</legend>
  <label for="name">Username</label>
  <input name="username" id="name">
  <label for="email">Email</label>
  <input name="email" type="email" id="email">
  <label for="password">Password</label>
  <input name="password" type="password" id="password">
  <button>Submit</button>
    </fieldset>
</form>

const form = document.querySelector("form")
form.addEventListener("submit", function (event){
event.preventDefault() // stops the form from putting the input in the URL and refresh the page, which is the default behaviour
const username = event.target.username.value;
const email = event.target.email.value;

const subs = document.getElementById("subs");
cont p = document.createElement("p");
p.textContent = `${username} with the email ${email} has requested contact.`
subs.appendChild(p)
})

## JS Events

const myButton = document.querySelector("button"); //takes a CSS rule and applies it to the HTML element we target. querySelector applies to the first item with the tag or class we are targeting. querySelectorAll bundles all tags into an array, so they can all be targeted together in the event.
console.dir(myButton) // console.dir shows item as object in console log

myButton.addEventListener("click", function(){ // the anonymous function is the callback function
myButton.classList.add("tomato") // adds the class to the object
myButton.classList.toggle("blueviolet") // adds the class to the object or removes the class if the object already has it
})

button {
padding: 1rem 2rem;
cursor: pointer;
}
.tomato {
background-color: tomato;
color: white;
font-family: monospace;
}
.blueviolet {
background-color: blueviolet;
color: white;
font-family: cursive;
}
<button>Click Me</button>
