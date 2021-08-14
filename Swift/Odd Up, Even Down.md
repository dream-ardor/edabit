## Odd Up, Even Down

Create a function that goes through the array, incrementing (+1) for each odd-valued number and decrementing (-1) for each even-valued number.
```swift
Examples
transform([1, 2, 3, 4, 5]) ➞ [2, 1, 4, 3, 6]

transform([3, 3, 4, 3]) ➞ [4, 4, 3, 4]

transform([2, 2, 0, 8, 10]) ➞ [1, 1, -1, 7, 9]
```


### 📑 My Code
```swift
let transform = {(a:[Int]) in a.map{$0 % 2 == 0 ? $0 - 1 : $0 + 1}}
```

