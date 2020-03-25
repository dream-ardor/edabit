## Video Length in Seconds

You are given the length of a video in minutes. The format is mm:ss (e.g.: "02:54"). Create a function that takes the video length and return it in seconds.
```ruby
Examples
minutes_to_seconds("01:00") ➞ 60

minutes_to_seconds("13:56") ➞ 836

minutes_to_seconds("10:60") ➞ false

Notes:

The video length is given as a string.
If the number of seconds is 60 or over, return false (see example #3).
You may get a number of minutes over 99 (e.g. "121:49" is perfectly valid).
```
### :gem: My Code
```ruby
def minutes_to_seconds(t)
  t.split(':')[1].to_i >= 60 ? false : t.split(':')[0].to_i * 60 + t.split(':')[1].to_i
end
```
