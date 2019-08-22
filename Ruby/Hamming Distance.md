## Hamming Distance
Hamming distance is the number of characters that differ between two strings.

To illustrate:

String1: "abcbba"
String2: "abcbda"

Hamming Distance: 1 - "b" vs. "d" is the only difference.
Create a function that computes the hamming distance between two strings.
```ruby
Examples
hamming_distance("abcde", "bcdef") ➞ 5

hamming_distance("abcde", "abcde") ➞ 0

hamming_distance("strong", "strung") ➞ 1
```
### :stars: My Code
```ruby
def hamming_distance(a, b)
  b_bytes = b.bytes
  a.each_byte.with_index.count {|x, i| x != b_bytes[i]}
end
```
