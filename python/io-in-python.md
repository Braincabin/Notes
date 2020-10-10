## IO in python

- [IO in python](#io-in-python)
	- [Output](#output)
		- [Simple string](#simple-string)
		- [Multiple arguments to print](#multiple-arguments-to-print)
		- [Seperator when given multiple arguments](#seperator-when-given-multiple-arguments)
		- [Trailing character](#trailing-character)
		- [file argument](#file-argument)
	- [Input](#input)
		- [Recieve input](#recieve-input)
		- [Recieve number input](#recieve-number-input)
		- [Handling invalid number input](#handling-invalid-number-input)


### Output

#### Simple string
To simply output a string:
```python
print("You can put any text here!")
```

#### Multiple arguments to print
Passing multiple arguments to `print` will be print with a seperator:
```python
print("Hello,", name, "! You are", age, "years old")
```

#### Seperator when given multiple arguments
By default, all the arguments passed to `print` will be seperated by a space (' ').
To change this default space character:
```python
print("First", "Second", "Third", "Fourth", sep="\n") # The sep argument is the seperator used
```
Output:
> First <br>
> Second <br>
> Third <br>
> Fourth <br>

**Note:** \n is just the *newline* character

#### Trailing character
By default `print` will add a newline to the end everytime you call it, if you don't want a newline character at the end:
```python
print("Loading", end="") # end is the argument to change the default trailing character 
print("...", end="")
print("...", end="")
```

Output:
> Loading......

---

#### file argument
This argument requires a *file like* object to be given to it, the output will be *written* to this file like object

By default the file-like object is `sys.stdout`, hence it prints to the *standard output* (aka console)

Usage:

```python
with open('./file.txt', 'a') as f:
	print('Hello, file', file=f)
```

Let's break this down
-	`with open('./file.txt', 'a') as f` opens a file named `file.txt` within the current directory in *append* (add more content) mode
-	the `as f` part in the first line says the name to be used for the variable, so that we can use it in our code
-	`print('Hello, file', file=f)` *writes* the output to the file
-	since we use the `with` keyword, once the block ends, `f.close` is automatically *called* (`f.close()`)

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
