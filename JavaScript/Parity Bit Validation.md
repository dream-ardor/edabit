## Parity Bit Validation

Parity bits are used as very simple checksum to ensure that binary data isn't corrupted during transit. Here's how they work:

If a binary string has an odd number of 1's, the parity bit is a 1.
If a binary string has an even number of 1's, the parity bit is a 0.
The parity bit is appended to the end of the binary string.
Create a function that validates whether a binary string is valid, using parity bits.
```
Worked Example
validateBinary("10110010") ➞ true

// The last digit is the parity bit.
// 0 is the last digit.
// 0 means that there should be an even number of 1's.
// There are four 1's.
// Return true.
```
 ```js
Examples
validateBinary("00101101") ➞ true

validateBinary("11000000") ➞ true

validateBinary("11000001") ➞ false
  ```
### ☀️ My Code
  ```js
  let validateBinary = b => b.match(/1/g).length % 2 == 0;
  ```
