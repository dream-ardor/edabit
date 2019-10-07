## Match the Last Item
Create a function that takes an array of items and checks if the last item matches the rest of the array.
```js
Examples
matchLastItem(["rsq", "6hi", "g", "rsq6hig"]) ➞ true
// The last item is the rest joined.

matchLastItem([1, 1, 1, "11"]) ➞ false
// The last item should be "111".

matchLastItem([8, "thunder", true, "8thundertrue"]) ➞ true
```
### :kaaba: My Code
```js
const matchLastItem = a => {
  b = a.pop();
  return a.join('') === b;
}
```
