### Python operators 

- [Python operators](#python-operators)
  - [Mathematical operators](#mathematical-operators)
    - [+ Operator](#ullioperatorliul)
    - [- Operator](#ullioperatorliul-1)
    - [* Operator](#ullioperatorliul-2)

#### Mathematical operators

##### + Operator

-   adds two numbers (`int` or `float`, `complex`) and returns the value

    ```python
    1 + 2       # returns 3
    1 + 0.1     # returns 1.1
    0.1 + 0.1   # returns 0.2
    1 + 2j      # returns (1+2j)
    ```

-   concatenates two strings and returns the value

    ```python
    'Hello, ' + 'world!'    # returns 'Hello, world!' as one string
    ```

-   concatenates two lists **or** two tuples

    ```python
    [1, 2] + [3, 4]     # returns [1, 2, 3, 4]
    (9, 8) + (7, 6)     # returns (9, 8, 7, 6)
    ```

-   **does not** concatenate a `string` and number
-   **does not** merge `sets` or `dicts`

##### - Operator

-   subtracts two numbers and returns the value

    ```python
    1 - 2               # returns -1
    1 - 0.1             # returns 0.9
    0.1 - 0.1           # returns 0.0
    (2j+1) - (1j-0.1)   # returns (1.1+1j)
    ```

-   **does not** work on `strings`, `sets` and `dicts`

##### * Operator

-   multiplies two numbers and returns the output

    ```python
    3 * 4               # returns 12
    1 * 0.1             # returns 0.1
    0.5 - 0.5           # returns 0.25
    (4j-1) * (2-1j)     # returns (2+9j)
    ```

-   when used with a `string` and `int`, repeats the `string` that many times and returns it

    ```python
    3 * 'Hi!'       # returns 'Hi!Hi!Hi!'
    'Ok' * 2        # returns 'OkOk'
    ```

-   when used with a `list` and `int`, repeats the `list` that many times and returns it

    ```python
    3 * [1, 2]          # returns [1, 2, 1, 2, 1, 2]
    ['a', 'b'] * 2      # returns ['a', 'b', 'a', 'b']
    ```

-   **Does'nt work** on `sets`, `lists` and `dicts`