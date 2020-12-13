## City School Creating IDS

Many IDS (for emails or Google ID) are created using the person's name.

Create a function that will return a four-character ID using the person's first name and last name. The first character will be the first letter of the first name but in lowercase. The next three characters will be the first three characters of the last name, but the first letter will be capitalized and the other two will be in lower case.
```python
Examples

create_id("mary", "lamb") ➞ "mLam"

create_id("John", "SMITH") ➞ "jSmi"

create_id("mary", "smith") ➞ "mSmi"
```
### :snake: My Code
```python
create_id = lambda f,l:f[0].lower()+l.title()[:3]
```
