## Remove Every Vowel from a String

Create a function that takes a string and returns a new string with all vowels removed.
```python
Examples
remove_vowels("I have never seen a thin person drinking Diet Coke.")
➞ " hv nvr sn  thn prsn drnkng Dt Ck."

remove_vowels("We're gonna build a wall!")
➞ "W'r gnn bld  wll!"

remove_vowels("Happy Thanksgiving to all--even the haters and losers!")
➞ "Hppy Thnksgvng t ll--vn th htrs nd lsrs!"
```
### :computer: My Code
```python
remove_vowels = lambda t:''.join(a for a in t if a not in set('aeiouAEIOU'))	
```
