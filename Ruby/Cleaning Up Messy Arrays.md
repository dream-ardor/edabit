## Cleaning Up Messy Arrays

Create a function that takes an array. This array will contain numbers represented as strings.

Your function should split this array into two new arrays. The first array should contain only even numbers. The second only odd. Then, wrap these two arrays in one main array and return it.

Return an empty array if there are no even numbers, or odd.
```ruby
Examples
clean_up_array(["8"]) ➞ [[8], []]

clean_up_array(["11"]) ➞ [[], [11]]

clean_up_array(["7", "4", "8"]) ➞ [[4, 8], [7]]

clean_up_array(["9", "4", "5", "8"]) ➞ [[4, 8], [9, 5]]
```
### :gem: My Code
```ruby
def clean_up_array(a)
  a.map(&:to_i).partition(&:even?)
end
```
