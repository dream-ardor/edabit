## Vowel Replacer
Create a function replaces all the vowels in a string with a specified character.
```ruby
Examples
replace_vowels("the aardvark", "#") ➞ "th# ##rdv#rk"

replace_vowels("minnie mouse", "?") ➞ "m?nn?? m??s?"

replace_vowels("shakespeare", "*") ➞ "sh*k*sp**r*"
```
### :ballot_box_with_check:My Code
```ruby
def replace_vowels(str, ch) 
  str.gsub(/[aeiou]/i, ch)
end
```
