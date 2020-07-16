## You FAILEDPASSED the Exam


The challenge is to fix all of the bugs in this incredibly messy code, which the code in the image might've actually looked like (probably not)! The code given will output the same middle two lines as in the image shown above.

First parameter is the user's score.
Second parameter is the required score.
```js
Examples
gradePercentage("85%", "85%") ➞ "You PASSED the Exam"

gradePercentage("99%", "85%") ➞ "You PASSED the Exam"

gradePercentage("65%", "90%") ➞ "You FAILED the Exam"

gradePercentage("5%", "8%") ➞ "You FAILED the Exam"
```
```
Notes:
Note that inputs will be given as a string percentage number.
Maintain all capitalization.
Feel free to declutter and refactor code if it helps!
```
### :computer: My Code
```js
const gradePercentage = (u,p) => parseInt(u) >= parseInt(p) ? 'You PASSED the Exam' : 'You FAILED the Exam';
```
