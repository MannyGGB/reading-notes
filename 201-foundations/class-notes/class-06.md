# Class 06 (25/09/2023)

## DOM

- Document Object Model
- Methods == actions inside objects

## Object Literals

- We use curly brackets to define the object.
  let obj = {
  name: "Tim", --> we have the key and the value
  age: 28,
  favFood: "pizza"
  }
  obj.height = "very tall"; --> we can add extra keys and values to the object or change a previous value
  obj.name = "Rich"
  console.log(obj.name, obj.age) --> we can access the values inside the object with dot notation

  - Method is a function that belongs in an object (dot notation)
    let person = {
    name: "Tim",
    age: 28,
    favFood: ["pizza", "cereal"], --> we can have arrays as values
    pet: {name: "Brie", breed: "schnauzer"}, --> we can have objects inside objects
    speak: function(){ --> we can have functions
    console.log("Hello")
    }
    }
    person.speak() --> to access the function in the object
    console.log(person.favFood[1]) --> access one item in the array inside the object
    console.log(person.pet.breed) --> access a key inside the object (pet) inside the object (person)

    - Objects inside arrays
      let arr = [
      {name: "Tim",
      age: 28},
      {name: "Rich",
      age: 25}
      ]
      console.log(arr[0].name) --> to access the first index (name) in the objects

- this.
  let person = {
  name: "Tim",
  age: 28,
  favFood: ["pizza", "cereal"],
  pet: {name: "Brie", breed: "schnauzer"},
  speak: function(){
  console.log(`${this.name} says hello`) --> we use this.key to access a property from inside the object.
  }
  }
  person.speak() --> this prints "Tim says hello"

## DOM manipulation

Everything is an object, including the whole document. We use dot notation to access info in objects.

// change the "textContent" property of the element with the id of "trevor"
let trev = document.getElementById("trevor");
trev.textContent = "Trev the Soft" // here we are changing the name written on HTML because the id is link to h2 on HTML.

// create a new element and put it onto the page
let parent = document.getElementById("parent");
let child = document.createElement("p") //created a p tag on HTML
child.textContent = "Some words";

parent.appendChild(child); // append means add to the end

// here we gave an id to a div on HTML, and then we accessed that id on JS and added content inside the div
let barryDiv = document.getElementById("barry");
barryDiv.textContent = "Manilow";
console.log() shows this as a tag
console.dir() shows this as an object

- To link JS and HTML, add <script> tag to the head with the keyword defer after src before >, so it is loaded after the whole page has loaded.

- const is used with arrays and objects, and cannot be changed. You can change the properties and values inside.
- let is used with variables and can be assigned different values and change.

## Demo

const cat = {
name: "Trevor",
age: 2,
interests: ["Philosophy", "Bacon", "Fish", "Minimalism"],
image: "./images/trevor.png",
goodWithKids: true,
goodWithDogs: false,
goodWithCats: false,
breed: "ginger",
};
const kittenProfiles = document.getElementById("kittenProfiles");

const article = document.createElement("article");

const h2 = document.createElement("h2");
h2.textContent = cat.name;
article.appendChild(h2);

const p = document.createElement("p");
p.textContent = `${cat.name} is ${cat.age} months old.`;
article.appendChild(p);
const img = document.createElement("img");
img.src = cat.image;
img.setAttribute("alt", cat.name);
article.appendChild(img);

const ul = document.createElement("ul");
for (let i = 0; i < cat.interests.length; i++){
const li = document.createElement ("li");
li.textContent = cat.interests[i];
ul.appendChild(li);
}
article.appendChild(ul)
kittenProfiles.appendChild(article)
