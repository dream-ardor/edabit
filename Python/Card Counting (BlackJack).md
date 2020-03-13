## Card Counting (BlackJack)
In BlackJack, cards are counted with -1, 0, 1 values:
```python
2, 3, 4, 5, 6 are counted as +1
7, 8, 9 are counted as 0
10, J, Q, K, A are counted as -1

Create a function that counts the number and returns it from the list of cards provided.

Examples
count([5, 9, 10, 3, "J", "A", 4, 8, 5]) ➞ 1

count(["A", "A", "K", "Q", "Q", "J"]) ➞ -6

count(["A", 5, 5, 2, 6, 2, 3, 8, 9, 7]) ➞ 5
```
### :snake: My Code
```python
def count(d):
 a = [1 if c in {2,3,4,5,6} else -1 if c in {10,'J','Q','K','A'} else 0 for c in d]
 return sum(a)
```
