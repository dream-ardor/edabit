## Prefixes vs. Suffixes

Create two functions: is_prefix(word, prefix-) and is_suffix(word, -suffix).
```
is_prefix should return true if it begins with the prefix argument.
is_suffix should return true if it ends with the suffix argument.

Otherwise return false.

Examples:
is_prefix("automation", "auto-") ➞ true

is_suffix("arachnophobia", "-phobia") ➞ true

is_prefix("retrospect", "sub-") ➞ false

is_suffix("vocation", "-logy") ➞ false
```
### :gem: My Code
```ruby
def is_prefix(w, p)
 w.start_with?(p.gsub('-',''))
end

def is_suffix(w, s)
 w.end_with?(s.gsub('-',''))
end
```
