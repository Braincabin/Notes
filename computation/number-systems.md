## Number systems

- [Number systems](#number-systems)
  - [Different number bases](#different-number-bases)
  - [General method for base conversion](#general-method-for-base-conversion)
  - [Decimal to binary conversion](#decimal-to-binary-conversion)
  - [Python built-in functions](#python-built-in-functions)

### Different number bases

| Base name   | Description           |
| ----------- | --------------------- |
| Binary      | Base 2 number system  |
| Octadecimal | Base 8 number system  |
| Decimal     | Base 10 number system |
| Hexadecimal | Base 16 number system |

**Note:** Decimal is the number base system we use in our everyday lives.

| Number base | Digits                                         |
| ----------- | ---------------------------------------------- |
| Binary      | 0, 1                                           |
| Octadecimal | 0, 1, 2, 3, 4, 5, 6, 7                         |
| Hexadecimal | 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F |

### General method for base conversion

-   Let the base be n
-   Let values v<sub>1</sub>, v<sub>2</sub> of each position be p<sup>n</sup> where p is _0-indexed_ position from the right
-   Let face value of each position be f<sub>1</sub>, f<sub>2</sub>, and so on...
-   The number's value will be
    f<sub>1</sub>v<sub>1</sub> + f<sub>2</sub>v<sub>2</sub> ... for all digits

### Decimal to binary conversion

| Position | Value |
| :------: | :---: |
|    0     |   1   |
|    1     |   2   |
|    2     |   4   |
|    3     |   8   |
|    4     |  16   |
|    5     |  32   |
|    6     |  64   |
|    7     |  128  |

**Some things to note:**

-   Position is _0-indexed_
-   This table applies for _signed 8-bit integer_

Method:
-   Start from position 7
-   If the number is greater that the value of the position
    -   write a 1 in the answer
    -   subtract that value from your number
    -   go to the next position
-   If the number is smaller
    -   write a 0 in the answer
    -   go to the next position
-   After position 0 your remainder should be 0


---

### Python built-in functions

| Function name | Usage                                      |
| ------------- | ------------------------------------------ |
| bin           | Function to convert decimal to binary      |
| oct           | Function to convert decimal to octadecimal |
| hex           | Function to convert decimal to hexadecimal |

**Note:** Python's int class has built-in support for converting all bases to decimal.

To convert a number of say base 8 (Octa-decimal) to decimal (base 10):

```python
print(int('123', 8))
```

This will output 83.
The first argument is the number (as a string) in any base and the second optional argument is the base.
Without any second arguement `int` interprets the string as a base 10 number.
