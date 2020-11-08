## Coding Website Score Calculator

Imagine you run a website that presents users with different coding challenges in levels Easy, Medium, and Hard, where users get points for completing challenges. An Easy challenge is worth 5 points, a Medium challenge is worth 10 points, and a Hard challenge is worth 20 points.

Create a function that takes in the number of each challenge level a user has played and calculates the user's total number of points. Keep in mind that a user cannot complete negative challenges, so the function should return the string "invalid" if any of the passed parameters are negative.
```ruby
Examples
score_calculator(1, 2, 3) ➞ 85

score_calculator(1, 0, 10) ➞ 205

score_calculator(5, 2, -6) ➞ "invalid"
```
### :gem: My Code
```ruby
def score_calculator(e, m, h)
  [e,m,h].any?(&:negative?) ? 'invalid': (e*5) + (m*10) + (h*20)
end
```
