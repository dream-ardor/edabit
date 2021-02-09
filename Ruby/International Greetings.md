## International Greetings

Suppose you have a guest list of students and the country they are from, stored as key-value pairs in a hash.
```ruby
GUEST_LIST = {
"Randy" => "Germany",
"Karla" => "France",
"Wendy" => "Japan",
"Norman" => "England",
"Sam" => "Argentina"
}
```
Write a function that takes in a name and returns a name tag, that should read:
```ruby
"Hi! I'm [name], and I'm from [country]."

If the name is not in the hash, return:

"Hi! I'm a guest."

Examples:
greeting("Randy") ➞ "Hi! I'm Randy, and I'm from Germany."

greeting("Sam") ➞ "Hi! I'm Sam, and I'm from Argentina."

greeting("Monti") ➞ "Hi! I'm a guest."
```
### :gem: My Code
```ruby
GUEST_LIST = {
  "Randy" => "Germany", 
  "Karla" => "France", 
  "Wendy" => "Japan", 
  "Norman" => "England", 
  "Sam" => "Argentina"
}

def greeting(n)
  GUEST_LIST[n] ? "Hi! I'm #{n}, and I'm from #{GUEST_LIST[n]}." : "Hi! I'm a guest."
end
```
