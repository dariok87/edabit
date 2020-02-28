# Async operations don't always go as planned. When errors creep up we need to know how to handle them. We can pass the reject callback to our executor function to pass errors to our promise.

let promise = new Promise( (resolve, reject) => {
setTimeout(( ) => {
/_ something went wrong _/
reject('oops!')
}, 1000)
})
You can pass Error objects as well. Here we pass a simple string "oops!".

Challenge

Reject the promise with the simple string "It's not a dog!".

Notes

Check the Resources tab for more info on promises.

```javascript
let promise = new Promise(resolve => {
  let animal = "cat";
  setTimeout(() => {
    if (animal === "dog") {
      resolve("It's a dog!");
    }
    if (animal !== "dog") {
      reject("It's not a dog'");
    }
  }, 1000);
});
```
