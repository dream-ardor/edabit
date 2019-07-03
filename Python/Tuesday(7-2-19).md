## Return the Last Element in a List
Create a function that accepts a list and returns the last item in the list. The list can be either homogeneous or heterogeneous.
```python
Examples
getLastItem([1, 2, 3]) ➞ 3

getLastItem(["cat", "dog", "duck"]) ➞ "duck"

getLastItem([True, False, True]) ➞ True

getLastItem([7, "String", False]) ➞ False
```
### :hamburger:My Code
```python
def getLastItem(lst):
	return lst[-1];
```

## Is the Word Singular or Plural?
Create a function that takes in a word and determines whether or not it is plural. A plural word is one that ends in "s".
```python
Examples
is_plural("changes") ➞ True

is_plural("change") ➞ False

is_plural("dudes") ➞ True

is_plural("magic") ➞ False
```
### :pizza: My Code
```python
is_plural = lambda word: word.endswith("s");
```

## Find the Largest Number in a List
Create a function that takes a list of numbers. Return the largest number in the list.
```python
Examples
findLargestNum([4, 5, 1, 3]) ➞ 5

findLargestNum([300, 200, 600, 150]) ➞ 600

findLargestNum([1000, 1001, 857, 1]) ➞ 1001
```
### :fries: My Code
```python
findLargestNum = lambda nums: max(nums);
	
```

## Concatenating Two Integer Lists
Create a function to concatenate two integer lists.
```python
Examples
concat([1, 3, 5], [2, 6, 8]) ➞ [1, 3, 5, 2, 6, 8]

concat([7, 8], [10, 9, 1, 1, 2]) ➞ [7, 8, 10, 9, 1, 1, 2]

concat([4, 5, 1], [3, 3, 3, 3, 3]) ➞ [4, 5, 1, 3, 3, 3, 3, 3]
```
### :spaghetti: My Code
```python
concat = lambda lst1, lst2: lst1 + lst2;
```
## Find the Smallest Number in a List
Create a function that takes a list of numbers and returns the smallest number in the list.
```python
Examples
findSmallestNum([34, 15, 88, 2]) ➞ 2

findSmallestNum([34, -345, -1, 100]) ➞ -345

findSmallestNum([-76, 1.345, 1, 0]) ➞ -76

findSmallestNum([0.4356, 0.8795, 0.5435, -0.9999]) ➞ -0.9999

findSmallestNum([7, 7, 7]) ➞ 7
```
### :curry: My Code
```python
def findSmallestNum(lst):
	return min(lst);
```
## Compare Strings by Sum of Characters
Create a function that takes two strings as arguments and return either True or False depending on whether the total number of characters in the first string is equal to the total number of characters in the second string.
```python
Examples
comp("AB", "CD") ➞ True

comp("ABC", "DE") ➞ False

comp("hello", "edabit") ➞ False
```
### :meat_on_bone:My Code
```python
def comp(txt1, txt2):
	return len(txt1) == len(txt2);
```

## Convert Number to String of Dashes
Create a function that takes a number (from 1 - 60) and returns a corresponding string of hyphens.
```python
Examples
num_to_dashes(1) ➞ "-"

num_to_dashes(5) ➞ "-----"

num_to_dashes(3) ➞ "---"
```
### :fried_shrimp:My Code
```python
def num_to_dashes(num):
	return(num * '-');
```

## Slice of Pie
Create a function that determines whether or not it's possible to split a pie fairly given these three parameters:
```
Total number of slices.
Number of recipients.
How many slices each person gets.
The function will be in this form:
```
```python
equal_slices(total slices, no. recipients, slices each)
Examples
equal_slices(11, 5, 2) ➞ True
# 5 people x 2 slices each = 10 slices < 11 slices 

equal_slices(11, 5, 3) ➞ False
# 5 people x 3 slices each = 15 slices > 11 slices

equal_slices(8, 3, 2) ➞ True

equal_slices(8, 3, 3) ➞ False

equal_slices(24, 12, 2) ➞ True
```
### :bento: My Code
```python
equal_slices =  lambda total, people, each: total >= people * each;
	
```
## Check String for Spaces
Create a function that returns True if a string contains any spaces.
```python
Examples
has_spaces("hello") ➞ False

has_spaces("hello, world") ➞ True

has_spaces(" ") ➞ True

has_spaces("") ➞ False

has_spaces(",./!@#") ➞ False
```
### :sushi:My Code
```python
def has_spaces(txt):
	return " " in txt;
```

## Find the Smallest and Biggest Numbers
Create a function that accepts a list of numbers and return both the minimum and maximum numbers, in that order (as a list).
```python
Examples
minMax([1, 2, 3, 4, 5]) ➞ [1, 5]

minMax([2334454, 5]) ➞ [5, 2334454]

minMax([1]) ➞ [1, 1]
```
### :ramen: My Code
```python
def minMax(nums):
	return [min(nums),max(nums)];
```
