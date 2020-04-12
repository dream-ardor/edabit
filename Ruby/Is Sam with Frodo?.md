## Is Sam with Frodo?

Sam and Frodo need to be close. If they are side by side in the array, your function should return true. If there is a name between them, return false.
```ruby
Examples
middle_earth(["Frodo", "Sam", "Gandalf"]) ➞ true

middle_earth(["Frodo", "Saruman", "Sam"]) ➞ false

middle_earth(["Orc", "Sam", "Frodo", "Legolas"]) ➞ true

Notes:
No matter who comes first, the result must be true if Frodo and Sam are side by side.
There is only one Sam and one Frodo in the array.
```

### :gem: My Code
```ruby
def middle_earth(a)
 a.index('Frodo') - a.index('Sam') == 1 or a.index('Sam') - a.index('Frodo') == 1
end
```
