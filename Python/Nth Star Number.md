## Nth Star Number

Create a function that takes a positive integer and returns the nth "star number".

A star number is a centered figurate number a centered hexagram (six-pointed star), such as the one that Chinese checkers is played on.
```python
Examples
star_number(2) ➞ 13

star_number(3) ➞ 37

star_number(5) ➞ 121
```
### :star: My Code
```python
star_number = lambda n:6 * n * (n - 1) + 1
	
```
