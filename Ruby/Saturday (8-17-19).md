## Absolute Sum
Take an array of integers (positive or negative or both) and return the sum of the absolute value of each element.
```ruby
Examples
get_abs_sum([2, -1, 4, 8, 10]) ➞ 25

get_abs_sum([-3, -4, -10, -2, -3]) ➞ 22

get_abs_sum([2, 4, 6, 8, 10]) ➞ 30

get_abs_sum([-1]) ➞ 1
```
### :black_circle: My Code
```ruby
def get_abs_sum(a)
  a.map{|x|x.abs}.reduce(:+)
end
```

## Capitalize by ASCII
Create a function that takes a string as input and capitalizes a letter if it's ASCII code is even, and returns its lower case version if it's ASCII code is odd.
```ruby
Examples
ascii_capitalize("to be or not to be!") ➞ "To Be oR NoT To Be!"

ascii_capitalize("THE LITTLE MERMAID") ➞ "THe LiTTLe meRmaiD"

ascii_capitalize("Oh what a beautiful morning.") ➞ "oH wHaT a BeauTiFuL moRNiNg."
```
### :black_circle: My Code
```ruby
def ascii_capitalize(s) 
  s.chars.map{|x| x.even? ? x.upcase : x.downcase }.join
end
```

## Remove the First and Last Characters
Create a function that removes the first and last characters from a string.
```ruby
Examples
remove_first_last("hello") ➞ "ell"

remove_first_last("maybe") ➞ "ayb"

remove_first_last("benefit") ➞ "enefi"

remove_first_last("a") ➞ "a"
```
### :black_circle: My Code
```ruby
def remove_first_last(s)
  s.size <= 2 ? s : s[1..-2]
end
```

## Additive Inverse
A number added with its additive inverse equals zero. Create a function that returns an array of additive inverses.
```ruby
Examples
additive_inverse([5, -7, 8, 3]) ➞ [-5, 7, -8, -3]

additive_inverse([1, 1, 1, 1, 1]) ➞ [-1, -1, -1, -1, -1]

additive_inverse([-5, -25, 35]) ➞ [5, 25, -35]
```
### :black_circle: My Code
```ruby
def additive_inverse(a)
  a.map{|x| x * -1 }
end
```

## Fix The Spacing
Additional spaces have been added to a sentence. Return the correct sentence by removing them. All words should be separated by one space, and there should be no spaces at the beginning or end of the sentence.
```ruby
Examples
correct_spacing("The film   starts       at      midnight. ")
➞ "The film starts at midnight."

correct_spacing("The     waves were crashing  on the     shore.   ")
➞ "The waves were crashing on the shore."

correct_spacing(" Always look on    the bright   side of  life.")
➞ "Always look on the bright side of life."
```
### :black_circle: My Code
```ruby
def correct_spacing(s)
  s.split.join(' ')
end
```
## Remove Every Vowel from a String
Create a function that takes a string and returns a new string with all vowels removed.
```ruby
Examples
remove_vowels("I have never seen a thin person drinking Diet Coke.")
➞ " hv nvr sn  thn prsn drnkng Dt Ck."

remove_vowels("We're gonna build a wall!")
➞ "W'r gnn bld  wll!"

remove_vowels("Happy Thanksgiving to all--even the haters and losers!")
➞ "Hppy
Thnksgvng t ll--vn th htrs nd lsrs!"
```
### :black_circle: My Code
```ruby
def remove_vowels(s)
  s.gsub(/[aeiou]/i,'')
end
```


