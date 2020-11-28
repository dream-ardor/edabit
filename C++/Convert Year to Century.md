## Convert Year to Century

Write a function that takes a year and returns its corresponding century.
```c++
Examples
centuryFromYear(2005) ➞ 21

centuryFromYear(1950) ➞ 20

centuryFromYear(1900) ➞ 19
```
### :palm_tree: My Code
```c++
#define centuryFromYear(y)(y-1)/100+1
```
