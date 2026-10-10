PRACCTICAL: 1 
Aim: A) Write a Python program using various datatypes and check their types. 

Code:
# Different data types

name = "SAISH"
age = 18
height = 5.4
is_student = True
marks = [80, 85, 90]
subject = ("Python", "DS")

# Display values and their data types

print("Name:", name, "Type:", type(name))
print("Age:", age, "Type:", type(age))
print("Height:", height, "Type:", type(height))
print("Student:", is_student, "Type:", type(is_student))
print("Marks:", marks, "Type:", type(marks))
print("Subject:", subject, "Type:", type(subject))


Aim: B) Write a Python program to perform Input and Output operations (accept a message and display it).

Code:
message = input("Enter a message:SAISH P ")
print("You entered:", message)



Practical: 2
Aim:A)  Write a Python program to check whether an entered number is Armstrong or not using a while loop.

Code:
num = int(input("Enter a number: "))

original = num
result = 0

while num > 0:
    digit = num % 10
    result = result + digit ** 3
    num = num // 10

if result == original:
    print(original, "is an Armstrong number")
else:
    print(original, "is not an Armstrong number")


Aim: B) Write a Python program to demonstrate the use of break and continue statements in loops.

CODE:

print("Using break:")
for i in range(1, 7):
    if i == 4:
        break
    print(i)


print("\nUsing continue:")
for i in range(1, 8):
    if i == 3:
        continue
    print(i)



Practical: 3

Aim: A) Write a Python program to check whether a number is even or odd.

Code:

num = int(input("Enter a number: "))

if num % 2 == 0:
    print("Even Number")
else:
    print("Odd Number")


Aim: B) Write a Python program to find the largest among three numbers.    

Code:

a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))

if a >= b and a >= c:
    print("Largest number is:", a)
elif b >= a and b >= c:
    print("Largest number is:", b)
else:
    print("Largest number is:", c)



Practical: 4

Aim: A) Write a Python program to convert Celsius to Fahrenheit.

Code:

celsius = float(input("Enter temperature in Celsius: "))
fahrenheit = (celsius * 9/5) + 32
print("Temperature in Fahrenheit:", fahrenheit)


Aim: B) Write a Python program to make a simple calculator (addition, subtraction, multiplication, division).

Code:

a = float(input("Enter first number: "))
b = float(input("Enter second number: "))

print("Addition =", a + b)
print("Subtraction =", a - b)
print("Multiplication =", a * b)
print("Division =", a / b)



Practical: 5

Aim: A) Write a Python program to find HCF (GCD) of two numbers.

Code:

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
while num2 != 0:
    temp = num2
    num2 = num1 % num2
    num1 = temp
print("HCF (GCD) =", num1)


Aim: B) Write a Python program to convert a decimal number to binary, octal, and hexadecimal.

Code:

num = int(input("Enter a decimal number: "))
print("Binary =", bin(num))
print("Octal =", oct(num))
print("Hexadecimal =", hex(num))



Practical: 6

Aim: A) Write a Python program to add two numbers.

Code:

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
sum = num1 + num2
print("Sum =", sum)


Aim: B) Write a Python program to calculate the area of a triangle.

Code:

base = float(input("Enter base: "))
height = float(input("Enter height: "))
area = 0.5 * base * height
print("Area of triangle =", area)



Practical: 7

Aim: A) Python Program to Apply Indexing and Slicing on an Array.

Code:


numbers = [10, 20, 30, 40, 50]

print("First element:", numbers[0])
print("Third element:", numbers[2])

print("First three elements:", numbers[0:3])
print("Last three elements:", numbers[2:5])


Aim: B) Python Program to Add and Remove Elements from an Array.

Code:

numbers = [10, 20, 30]

print("Original array:", numbers)

numbers.append(40)
print("After adding 40:", numbers)

numbers.insert(1, 15)
print("After inserting 15:", numbers)

numbers.remove(30)
print("After removing 30:", numbers)

numbers.pop()
print("After removing last element:", numbers)



Practical: 8

Aim: A) Python Program to Demonstrate String Immutability and Multiline String.

CODE:

name = "Hello"
print("Original string:", name)

name = "Yellow"
print("New string:", name)

message = """Python is easy to learn.
Python is widely used.
Python is a popular programming language."""

print("\nMultiline string:")
print(message)


Aim: B) Python Program to Compare and Concatenate Two Strings.

CODE:

str1 = "Python"
str2 = "Python"

if str1 == str2:
    print("Both strings are equal")
else:
    print("Both strings are different")

first = "Hello"
second = "Python"

result = first + " " + second

print("Concatenated string:", result)



Practical: 9

Aim: A) Python Program to Remove Punctuation from a String.

CODE:

import string
text = "Hello, World! Python is easy."
result = ""
for char in text:
    if char not in string.punctuation:
        result = result + char
print("Original string:", text)
print("String without punctuation:", result)


Aim: B) Python Program to Check Whether a String is Palindrome or Not.

CODE:

text = input("Enter a string: ")
reverse = text[::-1]
if text == reverse:
    print("The string is a palindrome")
else:
    print("The string is not a palindrome")



Practical: 9    


Aim: A) Python Program to Swap Two Variables.

CODE:

a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print("Before swapping:")
print("a =", a)
print("b =", b)

a, b = b, a

print("After swapping:")
print("a =", a)
print("b =", b)


Aim: B) Python Program to Shuffle a Deck of Cards.

CODE:

import random

suits = ["Hearts", "Diamonds", "Clubs", "Spades"]
ranks = ["2", "3", "4", "5", "6", "7", "8", "9",
         "10", "Jack", "Queen", "King", "Ace"]

deck = []

for suit in suits:
    for rank in ranks:
        deck.append(rank + " of " + suit)

random.shuffle(deck)

print("Shuffled deck:")

for card in deck:
    print(card)


