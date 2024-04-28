---
type: note
tags: [Digital_Logic]
---
08/17/2022 17:03

  

## Decimal to [[Binary]]
Hard way
1. Divide number left of radix by 2 by long division
2. Remainders after each step is binary number in reverse
3. For right of radix, multiply [[Decimal]] by two until you get to 1. If ones place goes over one, drop value to left of radix. At end, ones place of each step is binary number in order

"Easy" way
1. Find the powers of two that add up to the decimal number
2. Put a 1 in those places in the binary number


---

## Decimal to [[Hexadecimal|Hex]]
Same as to binary but divide by 16
For right of radix, same as binary but multiply by 16 until integer is reached

---

## Binary to Hex
1. Divide binary number into groups of 4 starting from radix
2. Each group is one place in hex number
	1. If a group at the right or left end has less than 4 places, add zeros to the left or right respectively

---

## Any to Decimal
For a number in any base, the decimal equivalent $N$ is:
$$
N=a_{n-1}b^{n-1}+a_{n-2}b^{n-2}+\cdots+a_0b^0
$$
where
- $a$ = digit of number
- $n$ = number of digits in number
- $b$ = base number (ex. for octal  $b=8$)

>[!example]
>$653_8=6(8^2)+5(8)+3=427$