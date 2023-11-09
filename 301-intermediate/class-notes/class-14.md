# Class 14 (09/11/2023)

## Lab demo

- The endpoint url and the client url are completely unrelated, even if they use the same params (for example, /:id)
- Use http://[::1]localhost:8080 if there is a problem with Thunder Client

## Try and catch

- Try --> we use it for the intended purpose.
- Catch --> we use it to show an error message.

```
const myName = "Tim";
console.log(myName)
try {
myName = "Sam"
} catch(error) {
  console.log("This is an error.")
}
console.log(myName)
```

- The purpose of try and catch is for the error to show, but not to break the code. The last console.log still runs even if there is an error in the try.
- Show one error at a time.

## OAuth code along

- Check repo (https://github.com/MannyGGB/auth0-sample)
- Getting started guide (https://manage.auth0.com/dashboard/uk/dev-3gsxkriro0sphbx/)
