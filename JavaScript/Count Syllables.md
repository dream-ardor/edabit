## Count Syllables

Create a function that counts the number of syllables a word has. Each syllable is separated with a dash -.
```js
Examples:
numberSyllables("buf-fet") ➞ 2

numberSyllables("beau-ti-ful") ➞ 3

numberSyllables("mon-u-men-tal") ➞ 4

numberSyllables("on-o-mat-o-poe-ia") ➞ 6
```

## My Code
```js
//Using regex
const numberSyllables = word =>  {
let syllables = /[^aeiouy]*[aeiouy]+(?:[^aeiouy]*$|[^aeiouy](?=[^aeiouy]))?/gi;
return word.match(syllables).length;
}

//Short version using split and length functions
const numberSyllables = word => word.split('-').length;
```

## Analysis
Like most problems, there are multiples ways to approach this one. The quick and easy version utilizes the split() and length() functions to check for the dashes and count the syllables from there. 

I actually like the regex approach. It's far more complicated than the short version but it teaches you a few fundamentals about programming and JavaScript. We declare a varable "syllables" in which the regex chain checks for the following: 
```js
* First, zero or more consonants: [^aeiouy]*
* Then, one or more vowels: [aeiouy]+
 After that, zero or one of the following:
* Consonants, followed by the end of the word: [^aeiouy]*$
* A consonant (if it is followed by another consonant): [^aeiouy](?=[^aeiouy])
```

We then chain the match() and length() functions to search for the syllables and then return the numerical value.
