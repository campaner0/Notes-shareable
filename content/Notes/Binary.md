---
type: note
---
08/17/2022 16:56

  #Digital_Logic 

Binary is a base 2 number system which therefore uses two digits: $0$ and $1$. It is often denoted with a subscript 'B' after the number to avoid confusion with other number systems. (ex: $1101001_B$)

## Data Representation
Binary data is made up of bits, the smallest division of binary. These are the digits. A byte is a group of 8 bits, a half word is 16, a word is 32, and a double-word is 64.

### 1's Complement
The 1's complement is the bitwise inversion of the number. That is, each bit is flipped. 1s become 0s and 0s become 1s..

---
### 2's Complement
The 2's complement is the 1's complement plus 1. The sum of a binary number and its 2's complement is always $2^n$, where $n$ is the number of bits in the number

---
### Unsigned


---

### Signed


---
## Math

### Addition
Addition is the same as [[Decimal]]

---
### Subtraction
##### 1's Complement
For the 1's complement:
1. Subtract as normal, taking a 1 from the leftmost 0
2. Invert the number (1s become 0s, 0s become 1s)

This will give the correct answer minus 1

##### 2's Complement
The process is:
1. Take 2's complement of subtrahend
2. Add result to minuend
3. Take 2's complement of result, make neg

---

### Multiplication
Same as decimal