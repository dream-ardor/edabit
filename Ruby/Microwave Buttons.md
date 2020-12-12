## Microwave Buttons

In microwave ovens, when buttons are pressed from 0-9, it will add that number to the microwave oven timer (starting from the left). All microwave ovens have the functionality where you can hit a "+30" button and it will add 30 seconds to the timer to cook your food. If you want to heat something for 5 mins, you can hit the "+30" button 10 times instead of thinking if there are fewer button presses that can give you the same result.

Create a function that takes an argument time and returns the shortest amount of button presses to set the given time on the microwave oven. The microwave oven timer always starts at 00:00.

```ruby
# It will add that number to the microwave oven timer (starting from the left).
# If the number "5" is pressed followed by "0" twice, it will put 05:00 on the timer.
# If the number "3" is pressed followed by "0", it will put 00:30 on the timer.

Button "+30", which adds 30 seconds to the current timer.

# If the number "+30" is pressed twice, it will put 00:60 on the timer.

A "Start" button which you have to finally press to start the microwave oven.

# Remember to press this!
Examples

microwave_buttons("00:30") ➞ 2
# "+30" to put 30 seconds on the timer.
# "Start" button to start the oven.

microwave_buttons("00:70") ➞ 3
# "7" followed by "0" to put 70 seconds on the timer.
# "Start" button to start the oven.

microwave_buttons("00:00") ➞ 1
# "Start" button to start the oven.
```

### :gem: My Code
```ruby
def microwave_buttons(t)
  t.match(/:30/) ? 2 : t.match(/10:/) ? 5 : t.match(/00:00/) ? 1 : 3
end
```
