## Halloween Day

Create a function that takes date in the format yyyy/mm/dd as an input and returns "Bonfire toffee" if the date is October 31, else return "toffee".
```python
Examples

halloween("2013/10/31") ➞ "Bonfire toffee"

halloween("2012/07/31") ➞ "toffee"

halloween("2011/10/12") ➞ "toffee"
```
### :jack_o_lantern: My Code
```python
halloween = lambda d:'Bonfire toffee' if d[5:] == '10/31' else 'toffee'


#alternate solution
halloween = lambda d:"Bonfire " * (d[-5:]=="10/31") + "toffee"
```
