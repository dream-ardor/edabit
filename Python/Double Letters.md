## Double Letters

Create a function that takes a word and returns True if the word has two consecutive identical letters.
```python
Examples
double_letters("loop") ➞ True

double_letters("yummy") ➞ True

double_letters("orange") ➞ False

double_letters("munchkin") ➞ False
```
### :computer: My Code
```python
import re
double_letters = lambda w:bool(re.search(r'(.)\1', w))
```
