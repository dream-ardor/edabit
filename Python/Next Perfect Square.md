## Next Perfect Square

Mubashir needs your help to find next integral perfect square after the one passed as a parameter.

Create a function which takes a given number n and returns next integral perfect square number. Return None if the given number is not a perfect square.
```python
Examples
next_square(121) ➞ 144

next_square(625) ➞ 676

next_square(114) ➞ None
# 114 is not a perfect square
```
### 🐍  My Code
```python
next_square = lambda n:None if (n ** 0.5) % 1 else (n ** 0.5 + 1) ** 2

#alternate
def next_square(n):
  x = n**.5
  if x%1==0:
    return (x+1)**2
```
