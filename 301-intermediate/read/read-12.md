# Reading 12

(https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

- In your own words, describe what each group of status code represents:
  - 100’s = give information to the client.
  - 200’s = request is successful and has been accepted.
  - 300’s = request has been redirected because it could not be found in the expected location.
  - 400’s = client error codes for an invalid request.
  - 500’s = server erros codes.
- What is a status code 202? Request has been accepted, and it will be finish in the future(promise), as it is asynchronous.
- What is a status code 308? Permanent redirect where the resource will be located from now on.
- What code would you use if an update didn’t return data to a client? 204 content.
- What code would you use if a resource used to exist but no longer does? 410 gone.
- What is the ‘Forbidden’ status code? Client has no permission to access the resource, despite authorisation status.

(https://www.youtube.com/watch?v=fgTGADljAeg&t=2s)

- Why do we need to pull our MongoDB database string out of our server and put it into our .env? Because it contains our password, which allows access to our database. This way, our password won't be pushed into GitHub.
- What is middleware? Middleware is the software apps use to communicate with, for example, an API or a server. It's in the middle, in between two apps or systems.
- What does app.use(express.json()) do? It lets the database accept JSON as the language for the data inside the documents.
- What does the /:id mean in a route? It means it is a parameter that we can acccess with the method request.params. This parameter it is the information the user inputs after the endpoint slash.
- What is the difference between PUT and PATCH? PUT updates all the information about a particular item, whereas PATCH updates specific data, in this case, PATCH only updates information that the user is inputting.
- How do you make a default value in a schema? You can add a default key to the class object we are creating, whose value will be added when there is no other value attached to it. For example:

```
subscribeDate: {
  default: Date.now
}
```

If the subscribeDate is unknown, it will be replaced by the current date.

- What does a 500 error status code mean? There is an error on the server or database, which caused the request not to work.
- What is the difference between a status 200 and a status 201? 200 means everything was successful in general, and 201 means we are successful when we created a new object, which is more specific.
