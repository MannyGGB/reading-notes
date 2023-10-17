# Catch-up 02 (17/10/2023)

- JavaScript
  - "use strict" for best practice.
- Local Storage

  - Saved per domain.
  - The data is stored in JSON format (JavaScript Object Notation).
  - Theme preferences, shopping cart in website, form data, location.
  - If there is a method in an object, we lose it when it goes to local storage.
  - To remove a value from a key in local storage, you need to get the item from local storage, parse it, remove the value, stringify the object and put it back to local storage. This process is easier with databases.

- Demo
  let person1 = {
  name: "John Doe",
  age: 30,
  city: "London",
  hobbies: ["climbing", "juggling", "fighting"]
  };

let person2 = {
name: "Jane Doe",
age: 30,
city: "London",
hobbies: ["parkour", "paragliding", "boccia"]
};

let jsonString1 = JSON.stringify(person1);
let jsonString2 = JSON.stringify(person2);

localStorage.setItem("person1", jsonString1);
localStorage.setItem("person2", jsonString2);

let retrievePerson1 = JSON.parse(localStorage.getItem("person1"));
let retrievePerson2 = JSON.parse(localStorage.getItem("person2"));

localStorage.removeItem("person2");
localStorage.clear();
