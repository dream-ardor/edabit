## Valid Zip Code

Zip codes consist of 5 consecutive digits. Given a string, write a function to determine whether the input is a valid zip code. A valid zip code is as follows:
```ruby
Must only contain numbers (no non-digits allowed).
Must not contain any spaces.
Must not be greater than 5 digits in length.

Examples
is_valid("59001") ➞ true

is_valid("853a7") ➞ false

is_valid("732 32") ➞ false
```
### :gem: My Code
```ruby
def is_valid(z)
 !!z.match(/\b\d{5}\b/)
end
```
