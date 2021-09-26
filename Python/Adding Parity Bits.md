## Adding Parity Bits

Parity bits are used as very simple checksum to ensure that binary data isn't corrupted during transit. Here's how they work:
```
If a binary string has an odd number of 1s, the parity bit is a 1.
If a binary string has an even number of 1s, the parity bit is a 0.
The parity bit is appended to the end of the binary string.
Create a function that adds the correct parity bit to a binary string.

Worked Example:
add_parity_bit("1011011") ➞ "10110111"

# There are five 1s.
# Since five is odd, the parity bit should be a 1.
# Add the parity bit to the end of the string.
# Return the result.

Examples:
add_parity_bit("0010110") ➞ "00101101"

add_parity_bit("1100000") ➞ "11000000"

add_parity_bit("1111111") ➞ "11111111"
```
### 🐍 My Code
```python
add_parity_bit = lambda b:b + str(b.count("1") % 2)
	
```
