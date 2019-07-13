## Recursion: Sum
Write a function that recursively finds the sum of the first n natural numbers.
```ruby
Examples
sum(5) ➞ 15
// 1 + 2 + 3 + 4 + 5 = 15

sum(1) ➞ 1

sum(12) ➞ 78
```
### :golf:My Code
```ruby
def sum(n)
	return n == 1 ? 1 : n + sum(n-1)
end
```
