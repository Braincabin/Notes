To recieve input from the user in python:
```python
name = input("Please enter your name: ")
```

**Things to note:**
 - Input **always** returns a string
 - The input reading in stopped once the `Enter` key is pressed


To recieve a number as input, you can pipe `input` into `int` like so:
```
age = int(input("Please enter your age: "))
```
**Things to note:**
 - If the input from the user was not a valid number, this will throw an error.
     To handle any invalid input you can use:
     ```python
     age_input = input("Please enter your age: ")
     if not age_input.isnumeric():
         print("Invalid input for age")
         # Terminate program using exit() or ask again
     ```
