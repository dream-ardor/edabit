## Calculate Determinant of a 2x2 Matrix

Create a function to calculate the determinant of a 2 * 2 matrix. The determinant of the following matrix is: ad - bc:
```
[[a, b], [c, d]]
Examples

calc_determinant([
  [1, 2],
  [3, 4]
]) ➞ -2

calc_determinant([
  [5, 3],
  [3, 1]
]) ➞ -4

calc_determinant([
  [1, 1],
  [1, 1]
]) ➞ 0
```
### 🐍 My Code
```python
calc_determinant = lambda m:m[0][0] * m[1][1] - m[0][1] * m[1][0]
```
