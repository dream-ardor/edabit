How Many D's Are There?

Create a function that counts how many D's are in a sentence.
```c++
Examples
countDs("My friend Dylan got distracted in school.") ➞ 4

countDs("Debris was scattered all over the yard.") ➞ 3

countDs("The rodents hibernated in their den.") ➞ 3
```
### :leaves: My Code
```c++
int countDs(std::string s) {
  return std::count(s.begin(),s.end(),'d') + std::count(s.begin(),s.end(),'D');
}
```
