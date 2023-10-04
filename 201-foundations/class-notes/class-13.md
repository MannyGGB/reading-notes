# Class 13 (04/10/2023)

## Lab review

- chart and JS logic.

## Data persistance and Local Storage

- Local storage is commonly used to set preferences (light/dark mode) and simple configurations.
- Local storage is always there, even after the tab is closed.

localStorage.setItem("name", "tim") --> save data // name is the key, tim is the value

localStorage.getItem("name") --> using key to get the value

localStorage.removeItem("name") --> removes the key and vlaue from storage

localstorage.clear() --> removes everything from local storage

const list = ["Gladiator", "Galaxy Quest"];

local.Storage.setItem("movies", list); --> the storage will save the list as a string

## JSON

- JS Object Notation

- JSON.stringify() --> turns an object into JSON using the stringify method.

- JSON.parse() --> retrieves the info (that was a string) as an object.
