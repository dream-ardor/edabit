## Stuttering Function

Write a function that stutters a word as if someone is struggling to read it. The first two letters are repeated twice with an ellipsis ... and space after each, and then the word is pronounced with a question mark ?.
```ruby
Examples
stutter("incredible") ➞ "in... in... incredible?"

stutter("enthusiastic") ➞ "en... en... enthusiastic?"

stutter("outstanding") ➞ "ou... ou... outstanding?"
```
### :gem: My Code
```ruby
def stutter(w)
  "#{w[0,2]}... " * 2 + w + '?'
end
```
