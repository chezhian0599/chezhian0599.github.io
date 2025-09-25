# Learning Python From Bro Code 

## Augmented assignment operators

Today I learned about augmented assignment operators in python

```
friends = 0
friends +=1
```
+= is called as augmented assignment operator, it is same as friends = friends + 1
this augmented assignment operator helps us to write clean code


## program to compute circumference & area of a circle

```
import math

radius = float(input("Enter the radius of a circle:"))

circumference = 2 * math.pi * radius

area = math.pi * pow(radius,2)

print(f"circumference of circle is {round(circumference,2)} cm")

print(f"Area of circle is {round(area,2)}cm ^2")
```

## logic to calculate the hypotenuse of a right triangle
```
import math 

a = float(input("Enter the length of side A:"))
b = float(input("Enter the length of side B:"))

c = math.sqrt(pow(a,2) + pow(b,2))

print(f"length of side c is {c}")
```

## calculator app that perform (+,-,*,/)

```
operator = input("Enter the operator(+,-,*,/) ")

num1 = float(input("Enter the 1st number:"))
num2 = float(input("Enter the 2nd number:"))

if operator in ("+","-","*","/"):
    if operator == "+":
        result = num1 + num2
        print(result)
    elif operator == "-":
        result = num1 - num2
        print(result)
    elif operator == "*":
        result = num1*num2
        print(result)
    elif operator == "/":
        result = num1/num2
        print(result)
else:
    print(f"The {operator} is not a valid operator")
```

## weight converter, the idea is to create a logic that converts kg to pounds and vice versa
```
weight_to_convert = float(input("Enter the weight"))
unit = input("Kilogram or Pounds (K or L)? ")

if unit == "K":
    final_output = weight_to_convert * 2.20
    print(f"{weight_to_convert} Kg is equal to {final_output} Lbs")
elif unit =="L":
    final_output = weight_to_convert / 2.20
    print(f"{weight_to_convert} Lbs is equal to {final_output} Kg")
else:
    print(f"{unit} is not a valid unit")
```

# conditional Expressions

### Conditional Expressions are one line shortcuts for if-else statements

Example 

x if condition else y

If the condition evaluates to True 'x' will be returned else 'y' will be returned

Code Examples

```
Set_1
num = 0

print('Positive' if num >0 else 'Negative')

Set_2
even_or_odd = 4

print('Even' if even_or_odd%2 ==0 else 'Odd')

Set_3

user_role = 'Guest'

print('Full Access' if user_role =='Admin' else 'Limited Access')

set_4

a = 7
b = 9

max_num = print(a if a>b else b)
min_num = print(a if a<b else b)

```







