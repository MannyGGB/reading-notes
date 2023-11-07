# Class 12 (07/11/2023)

## Lab demo

- To change the "test" name in MongoDB, add the name you prefer at the end of the MongoDB string after the final slash.

## Creating (POST)

- Body parser --> add **app.use(express.json())** at the top of the server

## Deleting (DELETE)

- When adding the delete button, make sure there is an anonymous function in the onClick value, so there is not an infinite loop.

```
onClick={()=> deleteMovie(movie.\_id)}

```
