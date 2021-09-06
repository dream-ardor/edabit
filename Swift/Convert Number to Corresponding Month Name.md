## Convert Number to Corresponding Month Name
Create a function that takes a number (from 1 to 12) and returns its corresponding month name as a string. For example, if you're given 3 as input, your function should return "March", because March is the 3rd month.

```swift
Examples
monthName(3) ➞ "March"

monthName(12) ➞ "December"

monthName(6) ➞ "June"
```
### 📆 My Code
```swift
let monthName:(Int) -> String = {Calendar.current.monthSymbols[$0-1]}

or

func monthName(_ num: Int) -> String {
  return DateFormatter().monthSymbols[num - 1];
}
```
