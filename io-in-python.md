## IO in python

- [IO in python](#io-in-python)
  - [Output](#output)
  - [Input](#input)
    - [Recieve input](#recieve-input)
    - [Recieve number input](#recieve-number-input)
    - [Handling invalid number input](#handling-invalid-number-input)


### Output

```python
print("You can put any text here!")
```

### Input

#### Recieve input

To recieve input from the user in python:

```python
name = input("Please enter your name: ")
```

**Things to note:**

-   `input` **always** returns a string
-   The input reading in stopped once the `Enter` key is pressed

---

#### Recieve number input
To recieve a number as input, you can pipe `input` into `int` like so:

```python
age = int(input("Please enter your age: "))
```

**Things to note:**

-   If the input from the user was not a valid number, this will throw an error.

---

#### Handling invalid number input
To handle any invalid input you can use:

```python
age_input = input("Please enter your age: ")
if not age_input.isnumeric():
    print("Invalid input for age")
    # Terminate program using exit() or ask again
    exit()

age = int(age_input)
print("You are", age, "years old.")
```
