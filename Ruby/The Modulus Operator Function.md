## The Modulus Operator Function

Create a function that will work as the modulus operator % without using the modulus operator. The modulus operator is a way to determine the remainder of a division operation. Instead of returning the result of the division, the modulo operation returns the whole number remainder.
```
Examples
mod(5, 2) ➞ 1

mod(218, 5) ➞ 3

mod(6, 3) ➞ 0
```
### 💎 My Code
```ruby
def mod(a,b)
  a - ~~(a/b) * b
end
```
