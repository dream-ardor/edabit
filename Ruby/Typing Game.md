## Typing Game
You're in the midst of creating a typing game.

Create a function that takes in two arrays: the array of user-typed words, and the array of correctly-typed words and outputs an array containing 1s (correctly-typed words) and -1s (incorrectly-typed words).
```ruby
# Inputs:
User-typed: ["cat", "blue", "skt", "umbrells", "paddy"]
Correct: ["cat", "blue", "sky", "umbrella", "paddy"]

# Output: [1, 1, -1, -1, 1]
```
### :trident: My Code
```ruby
def correct_stream(u, c)
  u.zip(c).map{|x,y| x == y ? 1 : -1}
end
```
