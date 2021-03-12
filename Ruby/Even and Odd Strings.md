## Even and Odd Strings

Given a one word lowercase string txt, return another string such that even-indexed and odd-indexed characters are grouped and groups are space-separated.
```ruby
Examples
even_odd_string("mubashir") ➞ "mbsi uahr"
# Letters at even indexes = "mbsi"
# Letters at odd indexes = "uahr"
# Join both strings with a space

even_odd_string("edabit") ➞ "eai dbt"

even_odd_string("airforce") ➞ "aroc ifre"
```
### :gem: My Code
```ruby
def even_odd_string(t)
 a = t.chars.select.each_with_index {|_,i| i.even?}.join
 b = t.chars.select.each_with_index {|_,i| i.odd?}.join
 "#{a} #{b}" 
end

#alternate solution
def even_odd_string(txt)
  txt.scan(/(.)(.)?/).transpose.map(&:join) * ' '
end


```
