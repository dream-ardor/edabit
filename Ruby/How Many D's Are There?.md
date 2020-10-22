## How Many D's Are There?

Create a function that counts how many D's are in a sentence.
```ruby
Examples
count_d("My friend Dylan got distracted in school.") ➞ 4

count_d("Debris was scattered all over the yard.") ➞ 3

count_d("The rodents hibernated in their den.") ➞ 3
```
### :gem: My Code
```ruby
def count_d(s)
  s.downcase.count('d')
end
```
