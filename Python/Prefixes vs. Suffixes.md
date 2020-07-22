## Prefixes vs. Suffixes

Create two functions: is_prefix(word, prefix-) and is_suffix(word, -suffix).

is_prefix should return True if it begins with the prefix argument.
is_suffix should return True if it ends with the suffix argument.

Otherwise return False.
```python
Examples
is_prefix("automation", "auto-") ➞ True

is_suffix("arachnophobia", "-phobia") ➞ True

is_prefix("retrospect", "sub-") ➞ False

is_suffix("vocation", "-logy") ➞ False
```
### :snake: My Code
```python
is_prefix = lambda w,p:w.startswith(p.strip('-'))

is_suffix = lambda w,s:w.endswith(s.strip('-'))
```
