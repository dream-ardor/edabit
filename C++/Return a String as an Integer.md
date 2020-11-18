## Return a String as an Integer

Create a function that takes a string and returns it as an integer.
```c++
Examples
StringInt("6") ➞ 6

StringInt("1000") ➞ 1000

StringInt("12") ➞ 12
```
### :leaves: My Code
```c++
int StringInt(std::string s) {
  return stoi(s) ;
}
```
