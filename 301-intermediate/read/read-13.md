# Reading 13

(https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)

- Which HTTP method would you use to update a record through an API? We can update the data with PUT, which replaces all current data with the new input data.
- Which REST methods require an ID parameter? Update and delete require an id parameter to make sure that we target the specific data we want to update or delete without affecting the rest of entries in the database.

(https://www.youtube.com/watch?v=EzNcBhSv1Wo)

- What’s the relationship between REST and CRUD?
  CRUD stands for Create, Read, Update, Delete, which are the common operations done on databases to manage the data in them. REST stands for Representational State Transfer or some rules on building web services. RESTful services use HTTP methods which have a connection to the CRUD operations: Create --> POST, Read --> GET, Update --> PUT, and Delete --> DELETE.
- If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

1. **Set up your coding environment**: create your server folder and install all the libraries and node modules needed to build your API.
2. **Middleware**: import the necessary libraries from the node modules and add them to your server.js.
3. **Endpoints**: set up your server.js by creating endpoints to cover all HTTP methods (POST, GET, PUT, DELETE at least).
4. **Schema**: create a schema to say how the data should be stored in the database, which will be used to create new items to store.
5. **Test and debug**: make sure your HTTP methods perform the intended functionalities in their corresponding endpoints. Use try and catch to show error messages when there is a problem between server and database.
