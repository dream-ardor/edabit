## Transcribe To mRNA

Transcribe the given DNA strand into corresponding mRNA - a type of RNA, that will be formed from DNA after transcription. DNA has the bases A, T, G and C, while RNA has U in place of T and all of the other bases remains the same.
```js
Examples
dnaToRna("ATTAGCGCGATATACGCGTAC") ➞ "UAAUCGCGCUAUAUGCGCAUG"

dnaToRna("CGATATA") ➞ "GCUAUAU"

dnaToRna("GTCATACGACGTA") ➞ "CAGUAUGCUGCAU"

Notes:
Transcription is the process of making complementary strand.
A, T, G and C in DNA converts to U, A, C and G respectively in mRNA.
```
### :sunny: My Code
```js
const dnaToRna = d => [...d].map(a => a == 'A' ? 'U' : a == 'T' ? 'A'
 : a == 'G' ? 'C' : 'G').join('');
  
//alternate
const dnaToRna = d => [...d].map(a => a ==  'C' ? a.replace('C', 'G') :
 a ==  'G' ? a.replace('G', 'C') : a ==  'T' ? a.replace('T', 'A'):
 a.replace('A', 'U')).join('');
  
 //alternate
const dnaToRna = d  => {
  let p = {A: 'U', T: 'A', G: 'C', C: 'G'}
  return [...d].reduce((v, k) => v + p[k], '')
}
```
