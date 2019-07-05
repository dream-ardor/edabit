## Reverse a List
Write a function to reverse a list.
```python
Examples
reverse([1, 2, 3, 4]) ➞ [4, 3, 2, 1]

reverse([9, 9, 2, 3, 4]) ➞ [4, 3, 2, 9, 9]

reverse([]) ➞ []
```
### :fireworks:My Code
```python
def reverse(lst):
	lst.reverse()
	return lst
```
## Word Endings
Create a function that adds a string ending to each member in a list.
```python
Examples
add_ending(["clever", "meek", "hurried", "nice"], "ly")
➞ ["cleverly", "meekly", "hurriedly", "nicely"]

add_ending(["new", "pander", "scoop"], "er")
➞ ["newer", "panderer", "scooper"]

add_ending(["bend", "sharpen", "mean"], "ing")
➞ ["bending", "sharpening", "meaning"]
```

### :sparkler:My Code
```python
def add_ending(lst, end):
	return list(lst+end for lst in lst)
```

## Edaaaaabit
Write a function that takes an integer and returns a string with the given number of "a"s in Edabit.
```python
Examples
how_many_times(5) ➞ "Edaaaaabit"

how_many_times(0) ➞ "Edbit"

how_many_times(12) ➞ "Edaaaaaaaaaaaabit"
```
### :wind_chime:My Code
```python
def how_many_times(num):
	return "Ed" + "a"*num + "bit"
```

## Check if a String Contains only Identical Characters
Write a function that returns True if all characters in a string are identical and False otherwise.
```
Examples
is_identical("aaaaaa") ➞ True

is_identical("aabaaa") ➞ False

is_identical("ccccca") ➞ False

is_identical("kk") ➞ True
```
### :rice_scene:My Code
```python
is_identical = lambda s:s == len(s)* s[0]
```

## Additive Inverse
A number added with its additive inverse equals zero. Create a function that returns a list of additive inverses.
```python
Examples
additive_inverse([5, -7, 8, 3]) ➞ [-5, 7, -8, -3]

additive_inverse([1, 1, 1, 1, 1]) ➞ [-1, -1, -1, -1, -1]

additive_inverse([-5, -25, 35]) ➞ [5, 25, -35]
```
### :fire:My Code
```python
additive_inverse = lambda lst:[-i for i in lst]
```

## Sum of Cubes
Create a function that takes a list of numbers and returns the sum of its cubes.
```python
Examples
sum_of_cubes([1, 5, 9]) ➞ 855
# Since 1^3 + 5^3 + 9^3 = 1 + 125 + 729 = 855

sum_of_cubes([3, 4, 5]) ➞ 216

sum_of_cubes([2]) ➞ 8

sum_of_cubes([]) ➞ 0
```
### :tada:My Code
```python
sum_of_cubes = lambda n: sum(i**3 for i in n)
```
## Count Instances of a Character in a String
Create a function that takes two strings as arguments and returns the number of times the first string is found in the second string.
```python
Examples
char_count("a", "edabit") ➞ 1

char_count("c", "Chamber of secrets") ➞ 1

char_count("b", "big fat bubble") ➞ 4
```
### :confetti_ball:My Code
```python
char_count = lambda txt1, txt2:txt2.count(txt1)
```





