## Incorrect Import Statement

Published by Mubashir Hassan in JavaScript
completeregexstrings
When importing objects from a module in Python, the syntax usually is as follows:
```
from module_name import object
```
Given a string of an incorrect import statement, return the fixed string. All import statements will be the wrong way round.
```js
Examples

fixImport("import object from module_name") ➞ "from module_name import object"

fixImport("import randint from random") ➞ "from random import randint"

fixImport("import pi from math") ➞ "from math import pi"
```
### :leaves: My Code
```js
let fixImport = s => s.replace(/(.+) (from.+)/,`$2 $1`);
```
