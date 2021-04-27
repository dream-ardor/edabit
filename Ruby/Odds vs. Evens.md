## Odds vs. Evens

Given an integer, return "odd" if the sum of all odd digits is greater than the sum of all even digits. Return "even" if the sum of even digits is greater than the sum of odd digits, and "equal" if both sums are the same.
```ruby
Examples
odds_vs_evens(97428) ➞ "odd"
# odd = 16 (9+7)
# even = 14 (4+2+8)

odds_vs_evens(81961) ➞ "even"
# odd = 11 (1+9+1)
# even = 14 (8+6)

odds_vs_evens(54870) ➞ "equal"
# odd = 12 (5+7)
# even = 12 (4+8+0)
```
### 💎 My Code
```ruby
def odds_vs_evens(n)
  e = o = 0
  n.to_s.chars.each { |c| c.to_i.odd? ? o += c.to_i : e += c.to_i }
  e == o ? 'equal':  e > o ? 'even' : 'odd'
end

#alternate solution
def odds_vs_evens(n)
  a = n.to_s.split('').map(&:to_i).select(&:odd?).reduce(:+) || 0
  b = n.to_s.split('').map(&:to_i).select(&:even?).reduce(:+) || 0
  a > b ? 'odd' : b == a ? 'equal' : 'even'
end
```
