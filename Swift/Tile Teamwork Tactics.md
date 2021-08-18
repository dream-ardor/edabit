## Tile Teamwork Tactics

In a board game, a piece may advance 1-6 tiles forward depending on the number rolled on a six-sided dice. If you advance your piece onto the same tile as another player's piece, both of you earn a bonus.

Given you and your friend's tile number, create a function that returns if it's possible to earn a bonus when you roll the dice.
```swift
Examples
possibleBonus(3, 7) ➞ true

possibleBonus(1, 9) ➞ false

possibleBonus(5, 3) ➞ false

Notes
You cannot move backward (which is why example #3 doesn't work).
If you are already on the same tile, return false, as you would be advancing away.
Expect only positive integer inputs.
```
### 🌴 My Code
```swift
let possibleBonus = {$0 < $1 && $1 - $0 < 7}
```
