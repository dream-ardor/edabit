## Product Divisible By Sum?
Write a function that returns true if the product of an array is divisible by the sum of that same array.
```ruby
Examples
divisible[3, 2, 4, 2] ➞ false

divisible[4, 2, 6] ➞ true

divisible[3, 5, 1] ➞ false
```
### :trident: My Code
```ruby
def divisible(arr)
  arr.inject(:*) % arr.reduce(:+) == 0
end
```

## Get the File Extension
Write a function that maps files to their extension names.
```ruby
Examples
get_extension(["code.html", "code.css"]) 
➞ ["html", "css"]

get_extension(["project1.jpg", "project1.pdf", "project1.mp3"])
➞ ["jpg", "pdf", "mp3"]

get_extension(["ruby.rb", "cplusplus.cpp", "python.py", "javascript.js"])
➞ ["rb", "cpp", "py", "js"]
```
### :trident: My Code
```ruby
def get_extension(a)
  a.map{|x| x.split(".")[1]}
end
```

## How Many Vowels?
Create a function that takes a string and returns the number (count) of vowels contained within it.
```ruby
Examples
count_vowels("Celebration") ➞ 5

count_vowels("Palm") ➞ 1

count_vowels("Prediction") ➞ 4
```
### :trident: My Code
```ruby
def count_vowels(s)
  s.count("aeiou")
end
```
## Reverse the Case
Given a string, create a function to reverse the case. All lower-cased letters should be upper-cased, and vice versa.
```ruby
Examples
reverse_case("Happy Birthday") ➞ "hAPPY bIRTHDAY"

reverse_case("MANY THANKS") ➞ "many thanks"

reverse_case("sPoNtAnEoUs") ➞ "SpOnTaNeOuS"
```
### :trident: My Code
```ruby
def reverse_case(s)
  s.swapcase
end
```
