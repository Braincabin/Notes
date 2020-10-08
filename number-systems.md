## Number systems

### Different number bases

| Base name   | Description           |
|-------------|-----------------------|
| Binary      | Base 2 number system  |
| Octadecimal | Base 8 number system  |
| Decimal     | Base 10 number system |
| Hexadecimal | Base 16 number system |

**Note:** Decimal is the number base system we use in our everyday lives.


Number base	| Digits
 ---		| ---
Binary		| 0, 1
Octadecimal	| 0, 1, 2, 3, 4, 5, 6, 7
Hexadecimal	| 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

### General method for base conversion
 - Let the base be n
 - Let values v<sub>1</sub>, v<sub>2</sub> of each position be p<sup>n</sup> where p is *0-indexed* position from the right
 - Let face value of each position be f<sub>1</sub>, f<sub>2</sub>, and so on... 
 - The number's value will be
     f<sub>1</sub>v<sub>1</sub> + f<sub>2</sub>v<sub>2</sub> ... for all digits

### Decimal to binary conversion:

Position	|Value
----------------|-----
0		|1
1		|2
2		|4
3		|8
4		|16
5		|32
6		|64
7		|128

**Some things to note:**
 - Position is *0-indexed*
 - This table applies for *signed 8-bit integer*


---

### Python built-in functions:

Function name	| Usage
 ---		| ---
bin		| Function to convert decimal to binary
oct		| Function to convert decimal to octadecimal
hex		| Function to convert decimal to hexadecimal

**Note:** Python's int class has built-in support for converting all bases to decimal.

To convert a number of say base 8 (Octa-decimal) to decimal (base 10):
```python
print(int('123', 8))
```
This will output 83.
The first argument is the number (as a string) in any base and the second optional argument is the base. 
Without any second arguement `int` interprets the string as a base 10 number.
