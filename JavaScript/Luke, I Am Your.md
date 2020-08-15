## Luke, I Am Your ...

Luke Skywalker has family and friends. Help him remind them who is who. Given a string with a name, return the relation of that person to Luke.
```
Person	Relation
Darth Vader	father
Leia	sister
Han	brother in law
R2D2	droid

Examples
relationToLuke("Darth Vader") ➞ "Luke, I am your father."

relationToLuke("Leia") ➞ "Luke, I am your sister."

relationToLuke("Han" ) ➞ "Luke, I am your brother in law."
```
### :computer: My Code
```js
const relationToLuke = n => {
 let a = {'Darth Vader': 'father', 'Leia':'sister', Han':'brother in law','R2D2':'droid'};
 return `Luke, I am your ${a[n]}.`
}

//alternate
const relationToLuke = n =>
 n == 'Darth Vader' ?  "Luke, I am your father." :
 n == 'Leia' ?  "Luke, I am your sister." :
 n == 'Han' ?  "Luke, I am your brother in law.":"Luke, I am your droid.";
```
