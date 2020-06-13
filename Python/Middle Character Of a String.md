## Middle Character Of a String

Create a function that returns the middle character of the string.
```python
Examples
middle_character('balkot') ➞ 'l'

middle_character('himani') ➞ 'm'

middle_character('nepali') ➞ 'p'

middle_character('java') ➞ 'a'

middle_character('kane') ➞ 'a'

middle_character('stoned') ➞ 'o'
```
### :sunny: My Code
```python
middle_character = lambda t:t[(len(t)-1)//2]
```
