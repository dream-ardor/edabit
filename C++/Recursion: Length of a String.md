## Recursion: Length of a String

Write a function that returns the length of a string. Make your function recursive.
```c++
Examples
length("apple") ➞ 5

length("make") ➞ 4

length("a") ➞ 1

length("") ➞ 0
```
### :leaves: My Code
```c++
int length(const char* s) {
  if(*s == '\0')
  return 0;
  return 1 + length(s + 1);
}
```
