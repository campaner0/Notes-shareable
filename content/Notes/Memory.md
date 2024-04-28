---
type: note
tags: [Embeded_Systems]
---
01/11/2023 15:15

  

Computer memory is where the computer stores program data and instructions. From the perspective of software, the memory is simply an addressable array of bytes. This is why most instructions only deal with bytes, though bitwise operations are possible.

[[RAM]] is read/write memory, but does not keep data if power is lost. [[ROM]] is read only memory that keeps its data

## Memory Locations
Every location in memory has an address that is used to locate the data stored at that location. The smallest subdivision of data that gets an address is the byte, and each byte-space in memory has a unique address usually written as a [[Hexadecimal|Hex]] number. 

### Words and Halfwords
Therefore words take up four spaces and are refered to by the lowest address out of its four bytes. Words can only be stored at memory spaces that have an address that is a multiple or 4 (address mod 4 = 0).

>[!example]
>If two words are next to each other (sequential memory), and the first word has an address of 0x0000, the next would have an address of 0x0004

Similarly, halfwords can only be stored at mod 2 = 0 addresses and are referred to by their lowest address.

### Endianess
Memory may be stored with the most/least significant byte (not bit) at the lowest address of the data or at the highest. If the LSB is at the lowest address, it is called little endian, and if it is at the the highest, it is big endian. Endianess is the order of bytes, but bit order within bytes is not affected. ARM is little endian by default but can be made big endian with config.

>[!note]
>Word addresses are defined by the lowest byte address regardless of endianess.

>[!example]
>For the data and addresses:
>|Address | Data|
>|---- | ----|
>|0x20008003|0xA7|
>|0x20008002|0x90|
>|0x20008001|0x8C|
>|0x20008000|0xEE|
>
>Big endian: 0xEE8C90A7
>Little endian: 0xA7908CEE

