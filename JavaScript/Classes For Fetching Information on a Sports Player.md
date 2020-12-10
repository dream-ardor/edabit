## Classes For Fetching Information on a Sports Player

Create a class that takes the following four arguments for a particular football player:
```
name
age
height
weight

Also, create three functions for the class that returns the following strings:

getAge() returns "name is age age"
getHeight() returns "name is heightcm"
getWeight() returns "name weighs weightkg"
Examples

 p1 = new Player("David Jones", 25, 175, 75)

 p1.getAge() ➞ "David Jones is age 25"
 p1.getHeight() ➞ "David Jones is 175cm"
 p1.getWeight() ➞ "David Jones weighs 75kg"
 ```
 ### My Code
 ```js
class Player {
	constructor(n,a,h,w){
	 this.n=n
	 this.a=a
	 this.h=h
	 this.w=w
	}
	getAge=()=>this.n+" is age "+this.a
	getHeight=()=>this.n+` is ${this.h}cm`
	getWeight=()=>this.n+` weighs ${this.w}kg`
}
 ```
