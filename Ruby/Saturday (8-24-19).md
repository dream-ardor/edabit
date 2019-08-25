## Generate a Countdown of Numbers in an Array
Create a function that takes a number as an argument and returns an array of numbers counting down from this number to zero.
```ruby
Examples
countdown(5) ➞ [5, 4, 3, 2, 1, 0]

countdown(1) ➞ [1, 0]

countdown(0) ➞ [0]
```
### :gear: My Code
```ruby
def countdown(s)
  [*0..s].reverse
end
```

## Amplify the Multiples of 4
Create a function that takes an integer and returns an array from 1 to the given number, where:

If the number can be divided evenly by 4, amplify it by 10 (i.e. return 10 times the number).
If the number cannot be divided evenly by 4, simply return the number.
```ruby
Examples
amplify(4) ➞ [1, 2, 3, 40]

amplify(3) ➞ [1, 2, 3]

amplify(25) ➞ [1, 2, 3, 40, 5, 6, 7, 80, 9, 10, 11, 120, 13, 14, 15, 160, 17, 18, 19, 200, 21, 22, 23, 240, 25]
```
### :gear: My Code
```ruby
def amplify(n)
  (1..n).map{|x|x % 4 == 0 ? x*10 : x }
end
```

## Repeating Letters N Times
Create a function that repeats each character in a string n times.
```ruby
Examples
repeat("mice", 5) ➞ "mmmmmiiiiiccccceeeee"

repeat("hello", 3) ➞ "hhheeellllllooo"

repeat("stop", 1) ➞ "stop"
```
### :gear: My Code
```ruby
def repeat(s, n)
  s.chars.map{|x| x * n}.join
end
```
## Lexicographically First and Last
Write a function that returns the lexicographically first and lexicographically last rearrangements of a string. Output the results in the following manner:

first_and_last(string) ➞ [first, last]
```
Examples
first_and_last("marmite") ➞ ["aeimmrt", "trmmiea"]

first_and_last("bench") ➞ ["bcehn", "nhecb"]

first_and_last("scoop") ➞ ["coops", "spooc"]
```
Notes
Lexicographically first: the permutation of the string that would appear first in the English dictionary (if the word existed).
Lexicographically last: the permutation of the string that would appear last in the English dictionary (if the word existed).

### :gear: My Code
```ruby
def first_and_last(s) 
  [s.chars.sort.join, s.chars.sort.reverse.join]
end
```

## Stretched Words
Write a function that takes a string, and returns a new string with any duplicate consecutive letters removed.
```ruby
Examples
unstretch("ppoeemm") ➞ "poem"

unstretch("wiiiinnnnd") ➞ "wind"

unstretch("ttiiitllleeee") ➞ "title"

unstretch("cccccaaarrrbbonnnnn") ➞ "carbon"
```
### :gear: My Code
```ruby
def unstretch(w)
  w.squeeze
end
```
## AlTeRnAtInG cApS
Create a function that alternates the case of the letters in a string.
```ruby
Examples
alternating_caps("Hello") ➞ "HeLlO"

alternating_caps("How are you?") ➞ "HoW aRe YoU?"

alternating_caps("OMG this website is awesome!") ➞ "OmG tHiS wEbSiTe Is AwEsOmE!"
```
### :gear: My Code
```ruby
def alternating_caps(s)
  s.gsub(/\w/).with_index{|x,y| y.even? ? x.upcase : x.downcase}
end
```
## Double Letters
Create a function that takes a word and returns true if the word has two consecutive identical letters.
```ruby
Examples
double_letters("loop") ➞ true

double_letters("yummy") ➞ true

double_letters("orange") ➞ false

double_letters("munchkin") ➞ false
```
### :gear: My Code
```ruby
def double_letters(w)
  (w=~ /(.)\1+/) != nil
end
```
