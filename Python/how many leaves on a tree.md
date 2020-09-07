how many leaves on a tree

make a function that will take a string which will either be big tree medium tree or a small tree and return how manny leaves there are on this big tree. on every branch there are N leaves. note :
```
a big tree has 100 branches

a medium tree has 50 branches

a small tree has 25 branches

Examples
how_many_leaves("big tree", 20) ➞ 2000
`100 * 20 = 2000`
how_many_leaves("medium tree", 30) ➞ 1500
`50 * 30 = 1500`
how_many_leaves("small tree", 27) ➞ 675
`25 * 27 = 675
```
### :snake: My Code
```python
how_manny_leaves = lambda t,n:{'b':100, 'm':50, 's':25}[t[0]]* n

#alternate solution
def how_manny_leaves(t,n):
  return n * 100 if t == 'big tree' else n*50 if t == 'medium tree' else n*25
  
#alternate soution 2
def how_manny_leaves(t,n):
  size = {'big tree':100, 'medium tree':50, 'small tree':25}
  return n * size[t]
```
