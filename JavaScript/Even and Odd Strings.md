## Even and Odd Strings
Given a string txt, return another string such that even-indexed and odd-indexed characters are grouped and groups are space-separated.
```js
Examples
evenOddString('mubashir') ➞ 'mbsi uahr'
// Alphabets at even indexes = 'mbsi'
// Alphabets at odd indexes = 'uahr'
// Join both strings with a space

evenOddString('edabit') ➞ 'eai dbt'

evenOddString('airforce') ➞ 'aroc ifre'
```
### :hibiscus: My Code
```js
const evenOddString = s => `${s.replace(/(.)./g, '$1')} ${s.replace(/.(.)?/g, '$1')}`;


//alternate solution
const evenOddString = s => `${s.replace(/./g, (s, a) => [s, ''][a & 1])} ${s.replace(/./g, (s, a) => ['', s][a & 1])}`;
```
