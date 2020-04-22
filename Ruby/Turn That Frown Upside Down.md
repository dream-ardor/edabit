## Turn That Frown Upside Down

It is important to be happy! Therefore, you must create a function that takes a sentence containing sad faces and turn them into happy ones! This involves changing only the mouths.
```
Sad face examples: :( 8( x( ;(
Happy face examples: :) 8) x) ;)
```
Make sure to only change the face if there are eyes before them, round(3.4) wouldn't become round)3.4) (for example).
```ruby
Examples
make_happy("My current mood: :(") ➞ "My current mood: :)"

make_happy("I was hungry 8(") ➞ "I was hungry 8)"

make_happy("print('x(')") ➞ "print('x)')"
```
### :gem: My Code
```ruby
def make_happy(str)
 str.gsub(/(?<=[:8x;])\(/, ")")
end

#longer version
def make_happy(s)
 s.gsub(':(',':)').gsub('8(','8)').gsub('x(','x)').gsub(';(',';)')
end
```
