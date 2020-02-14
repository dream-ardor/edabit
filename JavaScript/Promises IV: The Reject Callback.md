## Promises IV: The Reject Callback

Async operations don't always go as planned. When errors creep up we need to know how to handle them. We can pass the reject callback to our executor function to pass errors to our promise.
```js
let promise = new Promise( (resolve, reject) => {
  setTimeout(( ) => {
    /* something went wrong */
     reject('oops!')
  }, 1000)
})
```
You can pass Error objects as well. Here we pass a simple string "oops!".
```
Challenge
Reject the promise with the simple string "It's not a dog!".
```
### :computer: My Code
```js
let promise = new Promise( (resolve) => {
 let animal = "cat"
 setTimeout(() => {
  if(animal === "dog") {
  resolve("It's a dog!")
 } 
  if(animal !== "dog") {
  reject("It's not a dog!")
 }
}, 1000)
})
```
