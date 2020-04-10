## Simplified pigLatin

(Simplified) Rules for converting to pig latin: 1) Move the first alphabet to the back of the word 2) Add the substring 'ay' to the back
```python
simplePigLatin('pig') →  'igpay'
simplePigLatin('latin') →  'atinlay'
simplePigLatin('word') → 'ordway'
```
### :snake: My Code
```python
simplePigLatin = lambda w:w[1:]+w[0]+'ay'
```
