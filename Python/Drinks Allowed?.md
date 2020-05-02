## Drinks Allowed?

A bartender is writing a simple program to determine whether he should serve drinks to someone. He only serves drinks to people 18 and older and when he's not on break.

Given the person's age, and whether break time is in session, create a function which returns whether he should serve drinks.
```python
Examples
should_serve_drinks(17, True) ➞ False

should_serve_drinks(19, False) ➞ True

should_serve_drinks(30, True) ➞ False

Notes:
Return True or False.
Some countries have a slightly higher drinking age, but for the purposes of this challenge, it will be 18.
```
### :snake: My Code
```python
should_serve_drinks = lambda a,b: a >= 18 and b == False
```
