## Word Endings

Create a function that adds a string ending to each member in an array.
```c#
Examples
AddEnding(["clever", "meek", "hurried", "nice"], "ly")
➞ ["cleverly", "meekly", "hurriedly", "nicely"]

AddEnding(["new", "pander", "scoop"], "er")
➞ ["newer", "panderer", "scooper"]

AddEnding(["bend", "sharpen", "mean"], "ing")
➞ ["bending", "sharpening", "meaning"]
```
### 📘 My Code
```c#
using System.Linq;
class Program{public static string[] AddEnding(string[] a,string e) => a.Select(b => b + e).ToArray();}
```
