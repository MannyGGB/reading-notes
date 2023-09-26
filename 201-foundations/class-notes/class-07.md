# Class 07 (26/09/2023)

## Review DOM manipulation (lab 06)

## HTML Tables

<table>
  <tr>
    <th>Name</th>
    <th>Crisps</th>
    <th>Chocolate</th>
    <th>Drink</th>
  </tr>
  <tr>
    <td>Tim</td>
    <td>Knick Knacks</td>
    <td>Cadbury</td>
  <td>Juice</td>
  </tr>
  <tr>
  <td>Tim</td>
    <td>Knick Knacks</td>
    <td>Cadbury</td>
  <td>Juice</td>
    </tr>
</table>

table{
font-family: monospace;
}
tr:nth-child(odd){
background-color: antiquewhite;
}
tr:nth-child(even) {
background-color: lightblue;
}
th{
background-color: blue;
color: white;
padding: 8px;
}
td{
padding: 8px;
}

## Constructor function (creates objects) - Object-oriented Programming

function Kitten(name, age, interests, image, kids, dogs, cats, breed) { --> use capital letter for construct
this.name = name;
this.age = age;
this.interests = interests;
this.image = image;
this.goodWithKids = kids;
this.goodWithDogs = dogs;
this.goodWithCats = cats;
this.breed = breed;
}

Kitten.prototype.render = function() { --> render is not a keyword, can be changed
const kittenProfiles = document.getElementById("kittenProfiles");

const article = document.createElement("article");

const h2 = document.createElement("h2");
h2.textContent = this.name;
article.appendChild(h2);

const p = document.createElement("p");
p.textContent = `${this.name} is ${this.age} months old.`;
article.appendChild(p);

const img = document.createElement("img");
img.src = this.image;
img.setAttribute("alt", this.name);
article.appendChild(img);

const ul = document.createElement("ul");
for (let i = 0; i < this.interests.length; i++){
const li = document.createElement ("li");
li.textContent = this.interests[i];
ul.appendChild(li);
}
article.appendChild(ul)

kittenProfiles.appendChild(article)

}
const cat = new Kitten("Trevor", 2, ["Philosophy", "Bacon", "Fish", "Minimalism"],"./images/trevor.png", true, false, false,"ginger")

const cat2 = new Kitten("Phyllis", 10, ["mma", "krav maga", "podcasts", "karate"], "./images/phyllis.png", false, false, false, "tabby")

cat.render()
cat2.render()
