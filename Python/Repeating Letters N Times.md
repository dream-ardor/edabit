## Repeating Letters N Times

Create a function that repeats each character in a string n times.
```python
Examples
repeat("mice", 5) ➞ "mmmmmiiiiiccccceeeee"

repeat("hello", 3) ➞ "hhheeellllllooo"

repeat("stop", 1) ➞ "stop"
```
### :computer: My Code
```python
repeat = lambda a,n:''.join(i*n for i in a)
```
