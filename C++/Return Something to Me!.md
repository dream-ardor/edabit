## Return Something to Me!

Write a function that returns the string "something" joined with a space " " and the given argument a.
```c++
Examples
giveMeSomething("is better than nothing") ➞ "something is better than nothing"

giveMeSomething("Bob Jane") ➞ "something Bob Jane"

giveMeSomething("something") ➞ "something something"
```
### :leaves: My Code
```c++
#define giveMeSomething(a)std::string("something ") + a
```
