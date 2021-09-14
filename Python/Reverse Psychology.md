## Reverse Psychology

For this challenge, you will NOT be given a string. Your task isn't to add "Do not" before the given string. If there is no given string, you will not return "Do not do anything." Do not check the examples to know how to do this challenge.
```python
Examples
reverse_psychology("wash the dishes") ➞ "Do not wash the dishes."

reverse_psychology("eat your lunch") ➞ "Do not eat your lunch."

reverse_psychology("go to school") ➞ "Do not go to school."
```
### 🏗️ My Code
```python
reverse_psychology = lambda s = "do anything":"Do not " + s + "."
```
