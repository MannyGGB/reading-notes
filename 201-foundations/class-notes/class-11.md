# Class 11 (02/10/2023)

## Audio/Video

<audio id= "levees"> src= "" controls</audio>
autoplay: boolean (use sparingly)
controls: playback controls
loop: plays over and over again
muted: boolean, mute audio on page load
src: audio file/link
volume: range of 0.0(silent) to 1.0 (loud)
<button id= "randomiser">Randomise!</button> --> you can use id to interact with JS

const levees = document.getElementById ("levees");
const randomiser = document.getElementById ("randomiser")

randomiser.addEventListener("click", function(event) {}) etc

<video> src=""</video>
autoplay: boolean (use sparingly)
controls: playback controls
height: absolute value, no percentages
width: any value, including percentages
muted: boolean, mute audio on page load
poster: alternative image for thumbnail

## Array Methods

## CSS Grid

- \*{
  box-sizing: border-box;
  }

main {
width: 80%;
margin: 3rem auto;
}

.container {
border: 1px solid black;
display: grid;
grid-template-columns: 1fr 10% 1fr 40% ;
grid-template-rows: 14rem 3rem 6rem 6rem 6rem;
}

.container div {
background-color: grey;
margin: 0.5rem;
border: 1px solid black;
}

### Example of Flexbox

- \*{
  box-sizing: border-box;
  }

main {
width: 80%;
margin: 3rem auto;
}

.container {
border: 1px solid black;
display: flex;
}

.container div {
background-color: grey;
margin: 0.5rem;
border: 1px solid black;
flex: 1 1 20%;
}

div:nth-child(2) {
flex: 3 0 40%;
background-color: skyblue;
}

## Lab Demo

// DOM Nodes
let goatContainer = document.querySelector("section");
let image1 = document.querySelector("section img:first-child");
let image2 = document.querySelector("section img:nth-child(2)");

// keep each goat in an object
function Goat(name, src) {
this.name = name;
this.src = src;
this.views = 0;
this.clicks = 0;
}

// function to choose a random goat
function getRandomIndex() {
return Math.floor(Math.random() \* allGoats.length);
}

// function to render 2 random goats
function renderGoats() {
// get 2 rnadom indexes from our goat array
let goat1Index = getRandomIndex();
let goat2Index = getRandomIndex();

// prevent the two images being the same goat
while(goat1Index === goat2Index || goat1Index === goat3Index || goat2Index === goat3Index) {
goat2Index = getRandomIndex();
}

// change the src of our 2 images
image1.src = allGoats[goat1Index].src;
image2.src = allGoats[goat2Index].src;
image1.alt = allGoats[goat1Index].name;
image2.alt = allGoats[goat2Index].name;

// increase the goats views
allGoats[goat1Index].views++;
allGoats[goat2Index].views++;
}

// handle the goat being clicked
function handleGoatClick(event) {
// get the name of the goat we just clicked
let clickedGoat = event.target.alt;

// check if the click is on an image
if (event.target === goatContainer) {
alert("Please click on an image");
} else {
// render more goats
renderGoats();
}

// increase the clicks of the goat
// loop through allGoats
for (let i = 0; i < allGoats.length; i++) {
// check if the name of the goat in the array, matches the alt tag of our image
if (clickedGoat === allGoats[i].name) {
// increase the number of clicks
allGoats[i].clicks++;
// stop the for loop because we found the goat
break;
}
}
}

// make the goats
const allGoats = [
new Goat("Cruising Goat", "./images/cruisin-goat.jpg"),
new Goat("Float Your Goat", "./images/float-your-goat.jpg"),
new Goat("Goat Out of Hand", "./images/goat-out-of-hand.jpg"),
new Goat("Kissing Goat", "./images/kissing-goat.jpg"),
new Goat("Sassy Goat", "./images/sassy-goat.jpg"),
new Goat("Smiling Goat", "./images/smiling-goat.jpg"),
new Goat("Sweater Goat", "./images/sweater-goat.jpg"),
];

// render the results
// when the user clicks the view results button
// render a ul full of lis that tell the user how many tiems each goat has been clicked

// add the event listener to the goats
goatContainer.addEventListener("click", handleGoatClick);

renderGoats();
