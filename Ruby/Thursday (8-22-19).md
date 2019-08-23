## Reverse Words Starting With a Particular Letter
Write a function that reverses all the words in a sentence starting with a particular letter.
```ruby
Examples
special_reverse("word searches are super fun", "s")
➞ "word sehcraes are repus fun"

special_reverse("first man to walk on the moon", "m")
➞ "first nam to walk on the noom"

special_reverse("peter piper picked pickled peppers", "p")
➞ "retep repip dekcip delkcip sreppep"
```
### :flower_playing_cards: My Code
```ruby
def special_reverse(s, c)
  s.split.map{|x|x.start_with?(c) ? x.reverse : x}.join(' ')
end
```

## Transform Upvotes
Create a function that transforms a string of upvote counts into an array of numbers. Each k represents a thousand.
```ruby
Examples
transform_upvotes("6.8k 13.5k") ➞ [6800, 13500]

transform_upvotes("5.5k 8.9k 32") ➞ [5500, 8900, 32]

transform_upvotes("20.3k 3.8k 7.7k 992") ➞ [20300, 3800, 7700, 992]
```
### :flower_playing_cards: My Code
```ruby
def transform_upvotes(s)
  s.split.map{|x|x.include?('k') ? x.to_f * 1000 : x.to_i }
end
```

## Exists a Number Higher?
Write a function that returns true if there exists at least one number that is larger than or equal to n.
```ruby
Examples
exists_higher([5, 3, 15, 22, 4], 10) ➞ true

exists_higher([1, 2, 3, 4, 5], 8) ➞ false

exists_higher([4, 3, 3, 3, 2, 2, 2], 4) ➞ true

exists_higher([], 5) ➞ false
```
### :flower_playing_cards: My Code
```ruby
def exists_higher(a, n)
  a.any?{|x| x >= n}
end
```
## Chat Room Status
Write a function that returns the number of users in a chatroom based on the following rules:
```
If there is no one, return "no one online".
If there 1 person, return "[user1] online".
If there are 2 people, return [user 1] and [user 2] online".
If there are n>2 people, return the first two names and add "and n-2 more online".
For example, if there are 5 users, return: "[user1], [user2] and 3 more online"
```
```ruby
Examples
chatroom([]) ➞ "no one online"

chatroom(["paRIE_to"]) ➞ "parIE_to online"

chatroom(["s234f", "mailbox2"]) ➞ "s234f and mailbox2 online"

chatroom(["pap_ier44", "townieBOY", "panda321", "motor_bike5", "sandwichmaker833", "violinist91"])
➞ "pap_ier44, townieBOY and 4 more online"
```
### :flower_playing_cards: My Code
```ruby
def chatroomStatus(u)
  case u.size
   when 0
   "no one online"
   when 1
   "#{u[0]} online"
   when 2
   "#{u[0]} and #{u[1]} online"
   else
   "#{u[0]}, #{u[1]} and #{u.length-2} more online"
  end
end
```
## Upper or Lower Case
Return the smallest number of steps it takes to convert a string entirely into uppercase or entirely into lower case, whichever takes the fewest number of steps. A step consists of changing one character from lower to upper case, or vice versa.
```ruby
Examples
steps_to_convert("abC") ➞ 1
# "abC" converted to "abc" in 1 step

steps_to_convert("abCBA") ➞ 2
# "abCBA" converted to "ABCBA" in 2 steps

steps_to_convert("aba") ➞ 0

steps_to_convert("abaCCC") ➞ 3
```
### :flower_playing_cards: My Code
```ruby
def steps_to_convert(s)
  s.chars.partition{|x|x == x.downcase}.min_by(&:size).size
end
```
## Power of Two
Write a function that returns true if an integer is a power of 2, and false otherwise.
```ruby
Examples
power_of_two(32) ➞ true

power_of_two(1) ➞ true

power_of_two(18) ➞ false
```
### :flower_playing_cards: My Code
```ruby
def power_of_two(n)
  n.to_s(2).count('1') == 1
end
```






