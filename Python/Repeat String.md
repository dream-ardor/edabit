## Repeat String

Create a function that takes a string txt and a number n and returns the repeated string n number of times.

If given argument txt is not a string, return Not A String !!
```python
Examples
repeat_string("Mubashir", 2) ➞ "MubashirMubashir"

repeat_string("Matt", 3) ➞ "MattMattMatt"

repeat_string(1990, 7) ➞ "Not A String !!"
```
### :snake: My Code
```python
repeat_string = lambda t,n:t*n if type(t) is str else "Not A String !!"

```
