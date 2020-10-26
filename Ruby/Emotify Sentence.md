## Emotify Sentence

Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad and mad with their corresponding emoticons.
```ruby
word	emoticon
smile	:D
grin	:)
sad	:(
mad	:P

Examples:
emotify("Make me smile") ➞ "Make me :D"

emotify("Make me grin") ➞ "Make me :)"

emotify("Make me sad") ➞ "Make me :("
```
### :gem: My Code
```ruby
def emotify(s)
  s.sub('smile', ':D').sub('grin', ':)').sub('sad', ':(').sub('mad', ':P')
end
```
