***

# Learning Python Fundamentals

*(Inspired by Bro Code Tutorials)*

## Augmented Assignment Operators

Python supports augmented assignment operators, which help simplify code for updating variable values.
For example:

```python
friends = 0
friends += 1
```

Here, `+=` is the augmented assignment operator.
This is equivalent to:

```python
friends = friends + 1
```

These operators help write cleaner and more concise code.

***

## Program: Compute Circumference \& Area of a Circle

This program calculates the circumference and area for a given radius:

```python
import math

radius = float(input("Enter the radius of a circle: "))

circumference = 2 * math.pi * radius
area = math.pi * pow(radius, 2)

print(f"Circumference of circle is {round(circumference, 2)} cm")
print(f"Area of circle is {round(area, 2)} cm^2")
```


***

## Program: Calculate Hypotenuse of a Right Triangle

Use the Pythagorean theorem to find the hypotenuse:

```python
import math

a = float(input("Enter the length of side A: "))
b = float(input("Enter the length of side B: "))

c = math.sqrt(pow(a, 2) + pow(b, 2))
print(f"Length of side C is {c}")
```


***

## Simple Calculator App (+, -, *, /)

A basic calculator allowing user-chosen operations:

```python
operator = input("Enter the operator (+, -, *, /): ")

num1 = float(input("Enter the 1st number: "))
num2 = float(input("Enter the 2nd number: "))

if operator in ("+", "-", "*", "/"):
    if operator == "+":
        result = num1 + num2
    elif operator == "-":
        result = num1 - num2
    elif operator == "*":
        result = num1 * num2
    elif operator == "/":
        result = num1 / num2
    print(result)
else:
    print(f"{operator} is not a valid operator")
```


***

## Weight Converter: Kilograms ↔ Pounds

Convert between kilograms and pounds:

```python
weight = float(input("Enter the weight: "))
unit = input("Kilogram or Pounds (K or L)? ")

if unit == "K":
    result = weight * 2.20
    print(f"{weight} Kg is equal to {result} Lbs")
elif unit == "L":
    result = weight / 2.20
    print(f"{weight} Lbs is equal to {result} Kg")
else:
    print(f"{unit} is not a valid unit")
```


***

## Conditional Expressions (Ternary Operator)

Python allows concise conditional assignments and print statements using one-line if-else:

```python
# Example 1
num = 0
print('Positive' if num > 0 else 'Negative')

# Example 2
even_or_odd = 4
print('Even' if even_or_odd % 2 == 0 else 'Odd')

# Example 3
user_role = 'Guest'
print('Full Access' if user_role == 'Admin' else 'Limited Access')

# Example 4
a = 7
b = 9
print(a if a > b else b)  # Max
print(a if a < b else b)  # Min
```

Pattern: `x if condition else y`

***

## Username Validator Exercise

Check if a username meets specific conditions:

- Maximum 12 characters
- Only alphabetic letters
- No spaces or numbers

```python
def username_validator(username):
    if len(username) > 12:
        return "Total characters should not be more than 12"
    elif not username.isalpha():
        return "Your username cannot contain numbers"
    elif " " in username:
        return "Your username cannot contain spaces"
    else:
        return f"Welcome {username} !!"
```


***

## While Loop Example: User Input Validation

While loops execute code until a condition is no longer met:

```python
num = int(input("Enter a number between 1 and 10: "))

while num < 1 or num > 10:
    print("The entry is not valid")
    num = int(input("Enter a number between 1 and 10: "))

print(f"{num} is a valid number")
```


***

## Compound Interest Calculator (Two Approaches)

**Approach 1: Using Sequential While Loops**

```python
principal = 0
years = 0
interest = 0

while principal <= 0:
    print("Principal should be greater than 0")
    principal = int(input("Enter the principal (> 0): "))

while years <= 0:
    print("Years should be greater than 0")
    years = int(input("Enter the years (> 0): "))

while interest <= 0:
    print("Interest should be greater than 0")
    interest = int(input("Enter the interest (> 0): "))

total = principal * pow((1 + interest/100), years)
print(f"Balance after {years} year(s): ${total:.2f}")
```

**Approach 2: Using Infinite While Loops (`while True`)**

```python
while True:
    principal = int(input("Enter the principal (> 0): "))
    if principal > 0:
        break
    print("Principal cannot be less than 0")

while True:
    years = int(input("Enter the years (> 0): "))
    if years > 0:
        break
    print("Years cannot be less than 0")

while True:
    interest = int(input("Enter the interest (> 0): "))
    if interest > 0:
        break
    print("Interest should be greater than 0")

total = principal * pow((1 + interest/100), years)
print(f"Balance after {years} year(s): ${total:.2f}")
```


***

## Key Loop Concepts

- **Continue:**
Skips the current iteration if a certain condition is met.
- **Break:**
Immediately exits the loop if a certain condition is met.

***

This collection provides clean code snippets and essential Python logic fundamentals, ideal for beginners and anyone reviewing core concepts.
