## Instant JAZZ

Create a function which concantenates the number 7 to the end of every chord in a list. Ignore all chords which already end with 7.
```python
Examples
jazzify(["G", "F", "C"]) ➞ ["G7", "F7", "C7"]

jazzify(["Dm", "G", "E", "A"]) ➞ ["Dm7", "G7", "E7", "A7"]

jazzify(["F7", "E7", "A7", "Ab7", "Gm7", "C7"]) ➞ ["F7", "E7", "A7", "Ab7", "Gm7", "C7"]

jazzify([]) ➞ []
```
### :snake: My Code
```python
jazzify = lambda l:[x.strip('7')+ '7' for x in l]

#alternate solution
jazzify = lambda l: [k if '7' in k else k + '7' for k in l]
```
