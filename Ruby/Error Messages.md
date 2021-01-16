## Error Messages

Create a function that takes a number as an argument and returns the appropriate error message. You should do this without using the switch or if statements.

The input error will be 1 to 5:
```ruby
1 >> "Check the fan"
2 >> "Emergency stop"
3 >> "Pump Error"
4 >> "c"
5 >> "Temperature Sensor Error"

For any other value, return 101 (you can use an if statment here).

Examples
error(1) ➞ "Check the fan: e1"

error(2) ➞ "Emergency stop: e2"

error(3) ➞ "Pump Error: e3"
```
### :gem: My Code
```ruby
def error(n)
  n == 1 ? "Check the fan: e1" :
  n == 2 ?  "Emergency stop: e2" : 
  n == 3 ? "Pump Error: e3" :
  n == 4 ?  "c: e4" :
  n == 5 ? "Temperature Sensor Error: e5" : 101
end

#alternate solution
def error(n)
  hash = { 1 => 'Check the fan: e1', 
   2 => 'Emergency stop: e2',
   3 => 'Pump Error: e3', 
   4 => 'c: e4',
   5 => 'Temperature Sensor Error: e5' }
 hash[n] ||= 101
end
```
