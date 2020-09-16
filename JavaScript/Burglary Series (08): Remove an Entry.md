## Burglary Series (08): Remove an Entry

Your spouse tells you that one of the items on the list wasn't actually stolen, it is in your castle in Transilvania.

Given an object of the stolen items and an item name, return a copy without that item on the list.
```js
Examples
{ piano: 300, tv: 100, skate:50 } ➞ { piano: 300, tv: 100 }

{ mirror: 500, painting: 1 } ➞ { painting: 1 }

Notes:
The object will contain at least 2 items.
Preferably, mutate the copy not the original.
```
### :computer: My Code
```js
function removeEntry(obj, item) {
 const copy = {...obj};
 delete copy[item];
 return copy;
}
```
