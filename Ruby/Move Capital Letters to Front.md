## Move Capital Letters to the Front
Create a function that moves all capital letters to the front of a word.
```ruby
Examples
cap_to_front("hApPy") ➞ "APhpy"

cap_to_front("moveMENT") ➞ "MENTmove"

cap_to_front("shOrtCAKE") ➞ "OCAKEshrt"
```
### :snake: My Code
```ruby
def cap_to_front(s)
  (s.scan(/[A-Z]+/) << s.gsub(/[A-Z]/,'')).join
end
```
