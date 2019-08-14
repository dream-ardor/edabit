## International Greetings
Suppose you have a guest list of students and the country they are from, stored as key-value pairs in an object.
```js
const GUEST_LIST = {
  Randy: "Germany",
  Karla: "France",
  Wendy: "Japan",
  Norman: "England",
  Sam: "Argentina"
}
```
Write a function that takes in a name and returns a name tag, that should read:
```
"Hi! I'm [name], and I'm from [country]."
```
If the name is not in the object, return:
```
"Hi! I'm a guest."
```
```js
Examples
greeting("Randy") ➞ "Hi! I'm Randy, and I'm from Germany."

greeting("Sam") ➞ "Hi! I'm Sam, and I'm from Argentina."

greeting("Monti") ➞ "Hi! I'm a guest."
```

### :de:My Code
```js
const countries = {
	Randy: "Germany",
	Karla: "France",
	Wendy: "Japan",
	Norman: "England",
	Sam: "Argentina"
}

const greeting = name => countries.hasOwnProperty(name) ? 
`Hi! I'm ${name}, and I'm from ${countries[name]}.` : `Hi! I'm a guest.`
```
