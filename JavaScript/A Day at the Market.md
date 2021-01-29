## A Day at the Market

Backpack Bill and Wallet Will set off for the annual festival. As they approach the stalls, Bill retorts that he'll able to bring home more stuff than Will. Taking this as a challenge, Will refutes and a competition spurs into action.

Backpack Bill has an infinite inventory space, but a limited number of coins.
Wallet Will has an infinite number of coins, but a limited inventory space.
Create a function which returns the name of the man who can bring home the most items. The parameters are given as follows:
```js
Bill's amount of money.
Will's amount of inventory space.
The item's price.
The item's size.

Worked Example

whoWinsTonight(40, 95, 5, 10) ➞ 'Will'

# The item costs 5 coins and takes up 10 inventory spaces.
# Bill can only buy a maximum of 8 items (40 coins DIV 5 = 8).
# Will can only bring home a maximum of 9 items. (95 inventory spaces DIV 10 = 9).
# Will is the winner.

Examples

whoWinsTonight(20, 20, 5, 10) ➞ 'Bill'

whoWinsTonight(10, 2, 20, 1) ➞ 'Will'

whoWinsTonight(3, 7, 2, 5) ➞ 'Tie'

Notes

DIV means a floored division. That means you round down after dividing.
Return 'Tie' if both men can afford the same amount of stuff.
All numbers will be positive integers.
```
### :palm_tree:	 My Code
```js
const whoWinsTonight = (c,s,p,i) =>  {
  a = Math.floor(c/p), b = Math.floor(s/i);
  return a == b ? 'Tie' : a > b ? 'Bill' : 'Will';
}
```
