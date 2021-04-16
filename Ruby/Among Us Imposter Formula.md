## Among Us Imposter Formula

Create a function that calculates the chance of being an imposter. The formula for the chances of being an imposter is 100 × (i / p) where i is the imposter count and p is the player count. Make sure to round the value to the nearest integer and return the value as a percentage.
```ruby
Examples
imposter_formula(1, 10) ➞ "10%"

imposter_formula(2, 5) ➞ "40%"

imposter_formula(1, 8) ➞ "13%"

Notes
The player limit is 10 and the imposter count can only go up to 3.
```
### 💎 My Code
```ruby
def imposter_formula(i,p)
  "#{(100 * i/p.to_f).round}%"
end
```
