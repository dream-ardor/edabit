## How Many Unique Styles?

There are many different styles of music and many albums exhibit multiple styles. Create a function that takes an array of musical styles from albums and returns how many styles are unique.
```js
Examples
uniqueStyles([
  "Dub, Dancehall",
  "Industrial, Heavy Metal",
  "Techno, Dubstep",
  "Synth-pop, Euro-Disco",
  "Industrial, Techno, Minimal"
]) ➞ 9

uniqueStyles([
  "Soul",
  "House, Folk",
  "Trance, Downtempo, Big Beat, House",
  "Deep House",
  "Soul"
]) ➞ 7
```
### :computer: My Code
```js
const uniqueStyles = a => new Set(a.join().split(',')).size;
```
