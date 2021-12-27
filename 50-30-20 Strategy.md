## 50-30-20 Strategy

The 50-30-20 strategy is a simple way to budget, which involves spending 50% of after-tax income on needs, 30% after tax income on wants, and 20% after-tax income on savings or paying off debt.

Given the after-tax income as ati, what you are supposed to do is to make a function that will return a hash that shows how much a person needs to spend on needs, wants, and savings.
```
Examples
fifty_thirty_twenty(10000) ➞ { "Needs"=> 5000, "Wants"=> 3000, "Savings"=> 2000 }

fifty_thirty_twenty(50000) ➞ { "Needs"=> 25000, "Wants"=> 15000, "Savings"=> 10000 }

fifty_thirty_twenty(13450) ➞ { "Needs"=> 6725, "Wants"=> 4035, "Savings"=> 2690 }
```
### 💎 My Code
```ruby
def fifty_thirty_twenty(a)
  {"Needs" => a/2, "Wants" => a * 0.3, "Savings" => a * 0.2}
end
```
