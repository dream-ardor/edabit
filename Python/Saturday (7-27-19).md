## Edaaaaabit
Write a function that takes an integer and returns a string with the given number of "a"s in Edabit.
```python
Examples
how_many_times(5) ➞ "Edaaaaabit"

how_many_times(0) ➞ "Edbit"

how_many_times(12) ➞ "Edaaaaaaaaaaaabit"
```
### :ballot_box_with_check:My Code
```python
def how_many_times(num):
	return "Ed" + num * "a" + "bit"
```

## Is the Number Even or Odd?
Create a function that takes a number as an argument and returns "even" for even numbers and "odd" for odd numbers.
```python
Examples
isEvenOrOdd(3) ➞ "odd"

isEvenOrOdd(146) ➞ "even"
```
### :ballot_box_with_check:My Code
```python
def isEvenOrOdd(num):
	if num % 2 == 0:
	  return "even"
	else:
	  return "odd"
```

## Reverse the Case
Given a string, create a function to reverse the case. All lower-cased letters should be upper-cased, and vice versa.
```python
Examples
reverse_case("Happy Birthday") ➞ "hAPPY bIRTHDAY"

reverse_case("MANY THANKS") ➞ "many thanks"

reverse_case("sPoNtAnEoUs") ➞ "SpOnTaNeOuS"
```
### :ballot_box_with_check:My Code
```python
reverse_case = lambda txt:txt.swapcase()
```

## Count Syllables
Create a function that counts the number of syllables a word has. Each syllable is separated with a dash -.
```python
Examples
number_syllables("buf-fet") ➞ 2

number_syllables("beau-ti-ful") ➞ 3

number_syllables("mon-u-men-tal") ➞ 4

number_syllables("on-o-mat-o-poe-ia") ➞ 6
```
### :ballot_box_with_check:My Code
```python
def number_syllables(word):
	return len(word.split("-"))
```

## Reverse a List
Write a function to reverse a list.
```python
Examples
reverse([1, 2, 3, 4]) ➞ [4, 3, 2, 1]

reverse([9, 9, 2, 3, 4]) ➞ [4, 3, 2, 9, 9]

reverse([]) ➞ []
```
### :ballot_box_with_check:My Code
```python
reverse = lambda lst: lst[::-1]
```

## Find the Index (Part 1)
Create a function that finds the index of a given item.
```python
Examples
search([1, 5, 3], 5) ➞ 1

search([9, 8, 3], 3) ➞ 2

search([1, 2, 3], 4) ➞ -1
```
Notes
If the item is not present, return -1.
### :ballot_box_with_check:My Code
```python
search = lambda lst, item: lst.index(item) if item in lst else -1
```
## Find the Index
Create a function that takes a list and a string as arguments and return the index of the string.
```python
Examples
find_index(["hi", "edabit", "fgh", "abc"], "fgh") ➞ 2

find_index(["Red", "blue", "Blue", "Green"], "blue") ➞ 1

find_index(["a", "g", "y", "d"], "d") ➞ 3

find_index(["Pineapple", "Orange", "Grape", "Apple"], "Pineapple") ➞ 0
```
### :ballot_box_with_check:My Code
```python
find_index = lambda lst, txt: lst.index(txt)
```
## Missing Third Angle
You are given 2 out of 3 of the angles in a triangle, in degrees.

Write a function that classifies the missing angle as either "acute", "right", or "obtuse" based on its degrees.

An acute angle is one smaller than 90 degrees.
A right angle is one that is exactly 90 degrees.
An obtuse angle is one greater than 90 degrees (but smaller than 180 degrees).
For example: missing_angle(11, 20) should return "obtuse", since the missing angle would be 149 degrees, which makes it obtuse.
```python
Examples
missing_angle(27, 59) ➞ "obtuse"  # Since the missing

missing_angle(135, 11) ➞ "acute"

missing_angle(45, 45) ➞ "right"
```
### :ballot_box_with_check:My Code
```python
def missing_angle(a1, a2):
	if (a1 + a2) > 90:
	  return "acute"
	elif (a1 + a2) == 90:
	  return "right"
	else: 
	  return "obtuse"
```
