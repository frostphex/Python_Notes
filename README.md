# Python Notes

This repository contains essential Python programming concepts and notes, which can be handy for quick reference. These notes cover basic to intermediate Python topics, including variables, data types, conditional statements, functions, and more.

## Table of Contents
- [Getting Started](#getting-started)
- [User Input](#user-input)
- [Variables](#variables)
- [Data Types](#data-types)
  - [Integers](#integers)
  - [Floating Point Numbers](#floating-point-numbers)
- [Strings](#strings)
  - [Concatenation](#concatenation)
  - [f-Strings](#f-strings)
  - [Substrings and Slicing](#substrings-and-slicing)
- [Arithmetic Operations](#arithmetic-operations)
- [Conditional Statements](#conditional-statements)
- [Indentation](#indentation)
- [Loops](#loops)
  - [Initialization, Condition, and Update](#initialization-condition-and-update)
- [Functions](#functions)
- [Lists](#lists)
- [Debugging](#debugging)
- [Print Statement Formatting](#print-statement-formatting)

## Getting Started

Python programs consist of **commands** that instruct the computer to perform actions. Commands are executed sequentially, from top to bottom. 

For example:
```python
print("Hello, World!")
print(2 + 3)
```
- Use quotation marks (`"` or `'`) for strings to avoid `SyntaxError`.
- Perform arithmetic operations directly inside `print()`.

**Comments**: Use `#` to add comments that Python ignores during execution. For example:
```python
# This is a comment
print("This line will execute")
```

---

## User Input

To read input from a user, use the `input()` function:
```python
name = input("Enter your name: ")
print(f"Hello, {name}!")
```
- The input is always a string. Use `int()` or `float()` to convert it if necessary:
```python
age = int(input("Enter your age: "))
height = float(input("Enter your height: "))
```

---

## Variables

A **variable** is used to store data for later use. For example:
```python
x = 10
name = "Alice"
```
- Variables can store different data types, such as integers, strings, or lists.
- Variables can be named freely but should be descriptive.

### Naming Best Practices
- Use descriptive names (`age`, `total_price`), not vague ones (`a`, `x`).
- Follow the snake_case naming convention.

**Example:**
```python
price = 100
tax = 0.18
total_price = price + (price * tax)
print(f"Total price: {total_price}")
```

### String Concatenation
Combine strings using the `+` operator:
```python
greeting = "Hello, " + name
```
To combine strings and other data types, use `str()` or an f-string:
```python
age = 25
print("I am " + str(age) + " years old.")
# or
print(f"I am {age} years old.")
```

---

## Data Types

### Integers
Integers are whole numbers like `1`, `-15`, and `0`. They support basic arithmetic operations like addition, subtraction, multiplication, and division.

### Floating Point Numbers
Floating-point numbers are numbers with a decimal point (e.g., `3.14`, `-2.5`).

**Type Conversion**:
```python
x = int("42")  # Convert string to integer
y = float(3)    # Convert integer to float
```

---

## Strings

### Substrings and Slicing
Slicing allows you to extract parts of a string:
```python
my_string = "Python"
print(my_string[0:3])  # Output: Pyt
print(my_string[::-1])  # Output: nohtyP (reversed string)
```

---

## Arithmetic Operations

### Order of Operations
Use parentheses `()` to control the order of operations:
```python
result = (3 + 2) * 4  # Output: 20
```

---

## Conditional Statements

Conditional statements control the flow of your program based on conditions:
```python
if x > 10:
    print("x is greater than 10")
elif x == 10:
    print("x is 10")
else:
    print("x is less than 10")
```

---

## Indentation
Python uses indentation to define blocks of code. All lines in a block must have the same level of indentation:
```python
if x > 5:
    print("x is greater than 5")
    print("This is part of the same block")
```

---

## Loops

### Initialization, Condition, and Update
Loops have three parts:
1. **Initialization**: Set starting values.
2. **Condition**: Determine when to stop.
3. **Update**: Modify values during each iteration.

**For Loop Example:**
```python
for i in range(1, 6):
    print(i)
```
**While Loop Example:**
```python
count = 1
while count <= 5:
    print(count)
    count += 1
```

---

## Functions

Functions help organize and reuse code. Define a function using `def`:
```python
def greet(name):
    print(f"Hello, {name}!")

greet("Alice")
```

Avoid using global variables inside functions, as it may lead to bugs.

---

## Lists

Lists store multiple items in a single variable:
```python
my_list = [1, 2, 3, 4]
my_list.append(5)  # Add 5 to the end of the list
```

**Insert Example:**
```python
my_list.insert(2, 99)  # Insert 99 at index 2
```

---

## Debugging

**Tips:**
1. Use `print()` to check variable values during execution.
2. Break your program into smaller functions for easier debugging.
3. Test each function independently.

---

## Print Statement Formatting

Control print output with the `sep` and `end` arguments:
```python
print("A", "B", "C", sep="-")  # Output: A-B-C
print("Hello", end=" ")
print("World")  # Output: Hello World
```

**Format Numbers:**
```python
value = 1/3
print(f"Value: {value:.2f}")  # Output: Value: 0.33
```

---

These Python notes are a quick reference for common programming concepts. Add more examples and notes as you learn new topics!
