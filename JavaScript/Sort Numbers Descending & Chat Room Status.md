## Sort Numbers in Descending Order
Create a function that takes any nonnegative number as an argument and return it with it's digits in descending order. Descending order is when you sort from highest to lowest.
```js
Examples
sortDecending(123) ➞ 321

sortDecending(1254859723) ➞ 9875543221

sortDecending(73065) ➞ 76530
```
### :u5272:My Code
```js
const sortDecending = num => 
+num.toString().split('').sort(function(a,b){return b-a}).join('');
```
## Chat Room Status
Write a function that returns the number of users in a chatroom based on the following rules:
```
If there is no one, return "no one online".
If there 1 person, return "[user1] online".
If there are 2 people, return [user 1] and [user 2] online".
If there are n>2 people, return the first two names and add "and n-2 more online".
For example, if there are 5 users, return: "[user1], [user2] and 3 more online"
```
```js
Examples
chatroom([]) ➞ "no one online"

chatroom(["paRIE_to"]) ➞ "parIE_to online"

chatroom(["s234f", "mailbox2"]) ➞ "s234f and mailbox2 online"

chatroom(["pap_ier44", "townieBOY", "panda321", "motor_bike5", "sandwichmaker833", "violinist91"])
➞ "pap_ier44, townieBOY and 4 more online"
```
### :u6307:My Code
```js
function chatroomStatus(users) {
switch(users.length) {
  case 0: return "no one online"
  case 1: return users[0] + " online"
  case 2: return users[0] + " and " + users[1] + " online"
  default: return users[0] + ", " + users[1] + " and " +
  (users.length-2) + " more online"
}
}
```


