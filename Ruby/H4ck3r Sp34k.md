## H4ck3r Sp34k
Create a function that takes a string as an argument and returns a coded (h4ck3r 5p34k) version of the string.
```ruby
Examples
hacker_speak("javascript is cool") ➞ "j4v45cr1pt 15 c00l"

hacker_speak("programming is fun") ➞ "pr0gr4mm1ng 15 fun"

hacker_speak("become a coder") ➞ "b3c0m3 4 c0d3r"
```

### :gem: My Code
```ruby
def hacker_speak(s)
  s.gsub(/[aeios]/, 'a' => 4, 'e' => 3, 'i'=> 1, 'o' => 0, 's' => 5)
end
 
 #alternate
def hacker_speak(str)
  str.tr 'aeios', '43105'
end
```
