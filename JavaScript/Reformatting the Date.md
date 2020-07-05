## Reformatting the Date

Create a function that converts dates from one of five string formats:
```js
"January 9, 2019" (MM D, YYYY)
"Jan 9, 2019" (MM D, YYYY)
"01/09/2019" (MM/DD/YYYY)
"01-09-2019" (MM-DD-YYYY)
"01.09.2019" (MM.DD.YYYY)
```
The return value will be an array formatted like: [MM, DD, YYYY], where MM, DD, and YYYY are all integers. Using the examples above:
```js
Examples

convertDate("January 9, 2019") ➞ [1, 9, 2019]

convertDate("Jan 9, 2019") ➞ [1, 9, 2019]

convertDate("01/09/2019") ➞ [1, 9, 2019]

convertDate("01-09-2019") ➞ [1, 9, 2019]

convertDate("01.09.2019") ➞ [1, 9, 2019]
```
### :sunny: My Code
```js
const convertDate = d => {
 let a = new Date(d);
 return [a.getMonth()+1, a.getDate(), a.getFullYear()];
}
```
