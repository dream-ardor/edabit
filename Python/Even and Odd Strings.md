## Even and Odd Strings

Given a one word lowercase string txt, return another string such that even-indexed and odd-indexed characters are grouped and groups are space-separated.
```python
Examples

even_odd_string("mubashir") ➞ "mbsi uahr"
# Letters at even indexes = "mbsi"
# Letters at odd indexes = "uahr"
# Join both strings with a space

even_odd_string("edabit") ➞ "eai dbt"

even_odd_string("airforce") ➞ "aroc ifre"
```
### 🐍 My Code
```python
even_odd_string = lambda t:t[::2] + " " + t[1::2]
```
