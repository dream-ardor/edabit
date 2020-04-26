## Measure the depth of emptiness

In this challenge you will receive an input of the form

[[[[[[[[[[[]]]]]]]]]]]
i.e. a list containing a list containing a list containing .... a list containing nothing.

You goal is to measure the depth of this list, where [] has depth 1, [[]] has depth 2, [[[]]] has depth 3, etc.
```python
Examples
[] ➞ 1

[[]] ➞ 2

[[[]]] ➞ 3

[[[[[[[[[[[]]]]]]]]]]] ➞ 11

Notes
One way to do this is to use recursion. But maybe there's a way to just "count the brackets"?
```
### :snake: My Code
```python
measure_the_depth = lambda l:str(l).count('[')

```
