## Chinese Zodiac

Create a function that takes a year as an argument and returns the corresponding Chinese zodiac.
```js
Examples
chineseZodiac(2021) ➞ "Ox"

chineseZodiac(2020) ➞ "Rat"

chineseZodiac(1933) ➞ "Rooster"
```
### :mahjong:	My Code
```js
const chineseZodiac = y => ['Monkey', 'Rooster', 'Dog', 'Pig', 'Rat', 'Ox', 'Tiger', 
 'Rabbit','Dragon', 'Snake', 'Horse', 'Sheep'][y%12];
```
