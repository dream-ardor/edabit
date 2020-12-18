## Luke, I Am Your ...

Luke Skywalker has family and friends. Help him remind them who is who. Given a string with a name, return the relation of that person to Luke.
```c++
Person	    Relation
Darth Vader	 father
Leia	       sister
Han	         brother in law
R2D2        	droid

Examples

relationToLuke("Darth Vader") ➞ "Luke, I am your father."

relationToLuke("Leia") ➞ "Luke, I am your sister."

relationToLuke("Han") ➞ "Luke, I am your brother in law."
```
### :fallen_leaf: My Code
```c++
std::string relationToLuke(std::string n) {
  if (n == "Darth Vader") {return "Luke, I am your father.";}
  if (n == "Leia") {return "Luke, I am your sister.";}
  if (n == "Han") {return "Luke, I am your brother in law.";}
  if (n == "R2D2") {return "Luke, I am your droid.";}
}
```
