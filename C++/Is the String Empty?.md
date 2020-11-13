## Is the String Empty?

Create a function that returns true if a string is empty and false otherwise.
```c++ 
Examples
isEmpty("") ➞ true

isEmpty(" ") ➞ false

isEmpty("a") ➞ false

Notes:
A string containing only whitespaces " " does not count as empty.
Don't forget to return the result.
If you get stuck on a challenge, find help in the Resources tab.
If you're really stuck, unlock solutions in the Solutions tab.
```
### :leaves: My Code
```c++
#define isEmpty !~-sizeof

bool isEmpty(std::string str) {str.empty();}
```
