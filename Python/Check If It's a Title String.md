## Check If It's a Title String

Check if a text txt is a title text or not. A title text is one which has all the words in the text start with an upper case letter.
```python
Examples
check_title("A Mind Boggling Achievement") ➞ True

check_title("A Simple Java Script Program!") ➞ True

check_title("Water is transparent") ➞ False
```
### :evergreen_tree: My Code
```python
check_title = lambda t:t.title() == t
```
