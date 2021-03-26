## List From a Range of Numbers

Create a function that returns a list of all the integers between two given numbers start and end.
```python
Examples
range_of_num(2, 4) ➞ [3]

range_of_num(5, 9) ➞ [6, 7, 8]

range_of_num(2, 11) ➞ [3, 4, 5, 6, 7, 8, 9, 10]
```
### :snake: My Code
```python
range_of_num = lambda s,e:list(range(s+1, e))
```
