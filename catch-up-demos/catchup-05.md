# Catch-up 05 (19/10/2023)

## Objects and Constructors

let vampire = { // object literal
name: "Jane Doe",
age: 23232,
victims: [],
updateVictims: function(name, gallonsOfBlood){
this.victims.push({[name] : gallonsOfBlood})
}
}
console.log(vampire)
vampire.updateVictims("Sam", 24)

//constructed object
let zombie = new Object()

//arrow function --> don't use it in constructors or inside objects
const randomNum = () => {return.Math.floor(Math.random() \* 100)}

//constructor functions
let allShirts = [],

function TshirtsConstructor(price, color) {
this.price = price;
this.color = color;
this.type = "t-shirt";
allShirts.push(this)
}

let fineRed = new TshirtsConstructor(14.99, "red")
