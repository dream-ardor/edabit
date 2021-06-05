## Is the Word Singular or Plural?

Create a function that takes in a word and determines whether or not it is plural. A plural word is one that ends in "s".
```c#
Examples

IsPlural("changes") ➞ true

IsPlural("change") ➞ false

IsPlural("dudes") ➞ true

IsPlural("magic") ➞ false
```
### 📙 My Code
```c#
class Program {public static bool IsPlural(string w) => w.EndsWith("s");}
```
