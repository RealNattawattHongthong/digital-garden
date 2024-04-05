---
title: 3 - Paithong (Python)
---
# This is a simple Python program
# It prints "Hello, World!" to the console

print("Hello, World!")
# Variables and data types
name = "John"
age = 25
is_student = True

# Basic arithmetic operations
num1 = 10
num2 = 5
sum = num1 + num2
difference = num1 - num2
product = num1 * num2
quotient = num1 / num2

# Conditional statements
if age >= 18:
    print("You are an adult")
else:
    print("You are a minor")

# Loops
for i in range(5):
    print(i)

# Functions
def greet(name):
    print("Hello, " + name)

greet("Alice")
# Lists
fruits = ["apple", "banana", "orange"]
print(fruits[0])  # Output: apple
print(len(fruits))  # Output: 3

# Dictionaries
person = {"name": "John", "age": 25, "is_student": True}
print(person["name"])  # Output: John
print(person.get("age"))  # Output: 25

# File I/O
file = open("data.txt", "w")
file.write("Hello, World!")
file.close()

# Exception handling
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Error: Division by zero")

# Modules and libraries
import math
print(math.sqrt(16))  # Output: 4.0

# Classes and objects
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print("Hello, my name is " + self.name)

person = Person("Alice", 30)
person.greet()