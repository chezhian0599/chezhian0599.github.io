# operators in Python

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
