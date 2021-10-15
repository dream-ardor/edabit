## Rotate for Max Number

Create a function which takes a number and returns the maximum value by rearranging its digits.
```python
Examples
rotate_max_number(123) ➞ 321

rotate_max_number("001") ➞ 100

rotate_max_number(999) ➞ 999
```
### 🐍 My Code
```python
rotate_max_number = lambda n:int(''.join(sorted(str(n))[::-1]))
```
