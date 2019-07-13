## Word Endings
Create a function that adds a string ending to each member in an array.
```ruby
Examples
add_ending(["clever", "meek", "hurried", "nice"], "ly")
➞ ["cleverly", "meekly", "hurriedly", "nicely"]

add_ending(["new", "pander", "scoop"], "er")
➞ ["newer", "panderer", "scooper"]

add_ending(["bend", "sharpen", "mean"], "ing")
➞ ["bending", "sharpening", "meaning"]
```
### :gem:My Code
```ruby
def add_ending(arr, ending)
  return arr.map{ |arr| arr+ending }
end
```
