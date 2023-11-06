# Class 11 (06/11/2023)

## Morning Challenge

function evenNumbers(){
for(let i = 0; i <= 20; i+=2){
console.log(i)
}

}
evenNumbers()

for(let i = 0; i <= 20; i++){
if(i % 2 === 0){
console.log(i)
}
}

## MongoDB, Mongoose

- To connect our server to the MongoDB, we **npm i mongoose** in the server.
- package.json --> add a new line below "start" called **"dev": nodemon server.js**
  - this way, you can use npm run dev to start the server and client in their ports.
- After creating a password for your database, replace it in the Mongo string saved in the .env (remove <>)
  - Add the name of the project to the end of the database string.
- Mongoose is a class!

```
const mongoose = require("mongoose")
mongoose.connect(process.env.DATABASE_URL)

```

- **models** folder to define the schema in the database.

  ```
  const mongoose = require("mongoose");
  const {Schema} = mongoose;

  ```

- For our schema to be available, we need to **module.exports = Movie**
- Our seed.js is NOT the database; it only creates the data to be stored in the database.
  - **node seed** on terminal to create our array of objects.
