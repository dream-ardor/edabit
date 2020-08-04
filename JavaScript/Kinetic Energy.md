## Kinetic Energy

Kinetic energy can be calculated with the following formula:
```
KE = 1/2mv²

m is mass in kg
v is velocity in m/s
KE is kinetic energy in J
```
Return the Kinetic Energy in Joules, given the mass and velocity. For the purposes of this challenge, round answers to the nearest integer.
```js
Examples
kineticEnergy(60, 3) ➞ 270

kineticEnergy(45, 10) ➞ 2250

kineticEnergy(63.5, 7.35) ➞ 1715
```
### :computer: My Code
```js
const kineticEnergy = (m, v) => Math.round((m*0.5) * (v**2),1);
```
