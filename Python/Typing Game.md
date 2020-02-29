## Typing Game

You're in the midst of creating a typing game.

Create a function that takes in two lists: the list of user-typed words, and the list of correctly-typed words and outputs a list containing 1s (correctly-typed words) and -1s (incorrectly-typed words).
```python
# Inputs:
User-typed: ["cat", "blue", "skt", "umbrells", "paddy"]
Correct: ["cat", "blue", "sky", "umbrella", "paddy"]

# Output: [1, 1, -1, -1, 1]
Examples
correct_stream(
  ["it", "is", "find"],
  ["it", "is", "fine"]
) ➞ [1, 1, -1]

correct_stream(
  ["april", "showrs", "bring", "may", "flowers"],
  ["april", "showers", "bring", "may", "flowers"]
) ➞ [1, -1, 1, 1, 1]
```
### :snake: My Code
```python
def correct_stream(u, c):
  return [1 if i == j else -1 for i, j in zip(u, c)]
```
