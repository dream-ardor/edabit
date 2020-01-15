## Printer Levels

Given a dictionary of how many more pages each ink color can print, output the maximum number of pages the printer can print before any of the colors run out.
```python
Examples
ink_levels({
  "cyan": 23,
  "magenta": 12,
  "yellow": 10
}) ➞ 10

ink_levels({
  "cyan": 432,
  "magenta": 543,
  "yellow": 777
}) ➞ 432

ink_levels({
  "cyan": 700,
  "magenta": 700,
  "yellow": 0
}) ➞ 0
```
### :snake: My Code
```python
ink_levels = lambda i:min(i.values())
```
