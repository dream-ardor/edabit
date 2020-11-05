## Count Syllables

Create a function that counts the number of syllables a word has. Each syllable is separated with a dash -.

Examples
numberSyllables("buf-fet") ➞ 2

numberSyllables("beau-ti-ful") ➞ 3

numberSyllables("mon-u-men-tal") ➞ 4

numberSyllables("on-o-mat-o-poe-ia") ➞ 6

### :palm_tree: My Code
```c++
int numberSyllables(std::string w) {
 return count(w.begin(),w.end(),'-') + 1;
}
```
