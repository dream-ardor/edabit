## Movie Theatre Admittance

Write a function that checks whether a person can watch an MA15+ rated movie. One of the following two conditions is required for admittance:
```
The person is at least 15 years old.
They have parental supervision.
The function accepts two parameters, age and isSupervised. Return a boolean.
```
```c++
Examples
acceptIntoMovie(14, true) ➞ true

acceptIntoMovie(14, false) ➞ false

acceptIntoMovie(16, false) ➞ true
```
### :leaves: My Code
```c++
bool acceptIntoMovie(int a, bool i) {
  return a >= 15 | i;
}
```
