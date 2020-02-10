## Sort a List by String Length

Create a function that takes a list of strings and return a list, sorted from shortest to longest.
```python
Examples
sort_by_length(["Google", "Apple", "Microsoft"])
➞ ["Apple", "Google", "Microsoft"]

sort_by_length(["Leonardo", "Michelangelo", "Raphael", "Donatello"])
➞ ["Raphael", "Leonardo", "Donatello", "Michelangelo"]

sort_by_length(["Turing", "Einstein", "Jung"])
➞ ["Jung", "Turing", "Einstein"]
```
### :snake: My Code
```python
sort_by_length = lambda l: sorted(l,key=len)
```
