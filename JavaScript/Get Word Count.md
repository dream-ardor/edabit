## Get Word Count

Create a function that takes a string and returns the word count. The string will be a sentence.
```js
Examples:
countWords("Just an example here move along") ➞ 6

countWords("This is a test") ➞ 4

countWords("What an easy task, right") ➞ 5
```

## My Code
```js
const countWords = str => str.split(" ").length;
```
