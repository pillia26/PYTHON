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


