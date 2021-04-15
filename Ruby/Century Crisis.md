## Century Crisis

Scientists have discovered that in four decades, the world will EXPLODE! It will also take three decades to make a spaceship to travel to a new planet that can hold the entire world population.

You must calculate the number of people there will be in three decades from now.

The variable population is the world population now.
Assume that every month, someone gives birth to more people n.
Return the number of people there will be when the spaceship is complete.
```ruby
Examples
future_people(256, 2) ➞ 976

future_people(3248, 6) ➞ 5408

future_people(5240, 3) ➞ 6320
```
### 💎 My Code
```ruby
def future_people(p,n)
  p + 360 * n
end
```
