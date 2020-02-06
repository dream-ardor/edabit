## Video Length in Seconds

You are given the length of a video in minutes. The format is mm:ss (Example: '02:54'). Create a function which takes the video length and return it in seconds.
```js
Examples
minutesToSeconds('01:00') ➞ 60

minutesToSeconds('13:56') ➞ 836

minutesToSeconds('10:60') ➞ false
```
```
Notes
The video length is given as a string.
If the number of seconds is 60 or over, return false. (See Example #3).
You may get a number of minutes over 99 (Example: '121:49' is perfectly valid).
```
### :stopwatch: My Code
```js
const minutesToSeconds = t => 
 t.split(':')[1] >= 60 ? false :
 t.split(':').reduce((a,b) => (60 * a) + +b);
```
