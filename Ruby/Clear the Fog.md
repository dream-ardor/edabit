## Clear the Fog

Create a function which returns the word in the string, but with all the fog letters removed. However, if the string is clear from fog, return "It's a clear day!".
```ruby
Examples
clear_fog("sky") ➞ "It's a clear day!"

clear_fog("fogfogfffoooofftreesggfoogfog") ➞ "trees"

clear_fog("fogFogFogffffooobirdsandthebeesGGGfogFog") ➞ "birdsandthebees"
```
### :gem: My Code
```ruby
def clear_fog(s)
 s.include?('fog') ? s.tr('fog','') : 'It\'s a clear day!'
end
```
