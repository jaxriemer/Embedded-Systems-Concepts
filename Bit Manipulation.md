A solid understanding of Bitwise Operations is necessary for anyone working with embedded software. Being able to manipulate bits is important when trying to read out information from registers of a peripheral device, such as a temperature sensor. To understand how data is stored/outputted, the first step is to read through the datasheet of the sensor.

Recall: 1 byte has 8-bits

Some common bit operators are:

**NOT (~)**
This will flip a binary number. 1s become 0s, 0s become 1s.
ex: N = 10100100
  ~ N = 01011011

**AND (&)**
This compares two bit patterns of equal size. For each position, the bit of each pattern is compared. If both bits are 1, the resulting bit is 1. Otherwise it is 0.
ex:     A = 10011101
        B = 00110101
    A & B = 00010101

**OR (|)**
Similar to AND but if both bits are 0, the resulting bit is 0. Otherwise, it is 1.
ex:     A = 10011101
        B = 00110101
    A & B = 10111101

**XOR (^)**
If both bits are 0 or 1, the resulting bit is 0. Otherwise, it is 1.
ex:    A = 1001
       B = 1100
   A & B = 0101

**Left Shift (<<)**
This is the same as multiplying the pattern by $2^k$
ex:
      N = 1011
      N << 4 = 10110000

**Right Shift (>>)**
Same as dividing pattern by 2k.
ex:
      N = 1011
      N >> 2 = 10

Summary:

![Truth Table](https://github.com/jaxriemer/Embedded-Systems-Concepts/blob/main/images/TruthTable.png)

More in-depth information https://www.hackerearth.com/practice/basic-programming/bit-manipulation/basics-of-bit-manipulation/tutorial/
