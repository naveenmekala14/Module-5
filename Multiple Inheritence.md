# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
~~~
# Python program for Multiple Inheritance

# Base class 1
class Calculation1:

    def Summation(self, a, b):
        return a + b


# Base class 2
class Calculation2:

    def Subtraction(self, a, b):
        return a - b


# Derived class
class Derived(Calculation1, Calculation2):

    def Division(self, a, b):
        return a / b


# Get user input
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

# Create object
obj = Derived()

# Perform operations
print("\nAddition =", obj.Summation(num1, num2))
print("Subtraction =", obj.Subtraction(num1, num2))
print("Division =", obj.Division(num1, num2))
~~~
## Output Example
~~~
Enter first number: 20
Enter second number: 10

Addition = 30.0
Subtraction = 10.0
Division = 2.0
~~~
#Result 
The program is verified.
