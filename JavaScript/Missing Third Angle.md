## Missing Third Angle

You are given 2 out of 3 of the angles in a triangle, in degrees.

Write a function that classifies the missing angle as either "acute", "right", or "obtuse" based on its degrees.

* An acute angle is one smaller than 90 degrees.
* A right angle is one that is exactly 90 degrees.
* An obtuse angle is one greater than 90 degrees (but smaller than 180 degrees).
* For example: missingAngle(11, 20) should return "obtuse", since the missing angle would be 149 degrees, which makes it obtuse.

## My Code
```js
function missingAngle(angle1, angle2) {
	if (angle1 + angle2 < 90) {
		return "obtuse";
	}
	else if (angle1 + angle2 === 90) {
		return "right";
	}
	else  {
		return "acute";
	}
}

//Written in ES6
const missingAngle = (angle1, angle2) => {
	const angle3 = 180 - angle1 - angle2;
	return angle3 > 90 ? 'obtuse' : angle3 < 90 ? 'acute' : 'right'
	
}

```
