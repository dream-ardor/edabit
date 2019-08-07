## Shuffle the Name
Create a function that takes a string (will be a persons first and last name) and returns a string with the first and last name swapped.
```ruby
Examples
"Donald Trump" ➞ "Trump Donald"

"Rosie O'Donnell" ➞ "O'Donnell Rosie"

"Seymour Butts" ➞ "Butts Seymour"
```
### :gem:My Code
```ruby
def name_shuffle(str)
  str.split.reverse.join(' ')
end
```
