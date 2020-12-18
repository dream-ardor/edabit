## Modifying the Last Character

Create a function which makes the last character of a string repeat n number of times.
```c++
Examples

modifyLast("Hello", 3) ➞ "Hellooo"

modifyLast("hey", 6) ➞ "heyyyyyy"

modifyLast("excuse me what?", 5) ➞ "excuse me what?????"
```
### :leaves: My Code
```c++
std::string modifyLast(std::string s, int n) {
  while(--n) s += s.back();
  return s;
}
```
