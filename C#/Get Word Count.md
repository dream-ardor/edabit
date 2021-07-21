## Get Word Count

Create a function that takes a string and returns the word count. The string will be a sentence.
```c#
Examples
countWords("Just an example here move along") ➞ 6

countWords("This is a test") ➞ 4

countWords("What an easy task, right") ➞ 5
```
### 💻 My Code
```c#
class Program
{public static int CountWords(string s) => s.Split(' ').Length;}
```
