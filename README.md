# python-notes
20/02/25
print("jathin" + str(2001) + "@gmail.com")
variables: is a sequence of characters which stores different data values
print is function which performs a task
a = "jathin"
b = 2001
c = "@gmail.com"
print(a + str(b) + c)
/n escape sequence character:
Is a backslash followed by a character you want to insert
Data types:are needed to store different values in memory

Variable is like a container that holds data. Very similar to how our containers in kitchen holds sugar, salt etc Creating a variable

like creating a placeholder in memory and assigning it some value. In Python its as easy as writing:
String: Strings are sequences of characters and are treated as immutable in Python. They support a wide range of string manipulation operations.
Exception: Exceptions are types of errors that occur when the program is being executed and change the normal flow of the program
Data types: data types are needed to store different types of values in memory
It specifies type of value that variable holds
Data types are needed to do different operations without causing an error


There are inbuilt data types in python
They are:
Numerical datatype
Int
Float
Complex
Boolean: true or false 
List:collect of different items enclosed between square brackets which we can’t change the values
Tuple: tuple is a collection of different elements which we can change the values
Dictionary:collection of key value elements 
Represents values of key elements
codes with same output by using different datatypes in python:
email_str = "jathin2001@gmail.com"

email_list = list(email_str)
email_tuple = tuple(email_str)
email_set = sorted(set(email_str))
email_dict = {index: char for index, char in enumerate(email_str)}
email_bytes = email_str.encode('utf-8')
email_bytearray = bytearray(email_bytes)
email_bool = "@" in email_str
email_int = sum(ord(char) for char in email_str)
email_float = float(email_int)
email_complex = complex(email_int, len(email_str))

print("String:", email_str)
print("List:", "".join(email_list))
print("Tuple:", "".join(email_tuple))
print("Set:", "".join(email_set))
print("Dictionary:", "".join(email_dict.values()))
print("Bytes:", email_bytes.decode('utf-8'))
print("Bytearray:", email_bytearray.decode('utf-8'))
print("Boolean:", email_str if email_bool else "Invalid email")
print("Integer:", email_str)
print("Float:", email_str)
print("Complex:", email_str)
>PROGRAM TO PRINT CAPITALS OF INDIAN STAES using DICTIONARY data type
states_capitals = {"STATE": "CAPITALS", "Andhra Pradesh": "Amaravati", "Arunachal Pradesh": "Itanagar", "Assam": "Dispur",
    "Bihar": "Patna", "Chhattisgarh": "Raipur", "Goa": "Panaji", "Gujarat": "Gandhinagar",
    "Haryana": "Chandigarh", "Himachal Pradesh": "Shimla", "Jharkhand": "Ranchi",
    "Karnataka": "Bengaluru", "Kerala": "Thiruvananthapuram", "Madhya Pradesh": "Bhopal",
    "Maharashtra": "Mumbai", "Manipur": "Imphal", "Meghalaya": "Shillong",
    "Mizoram": "Aizawl", "Nagaland": "Kohima", "Odisha": "Bhubaneswar",
    "Punjab": "Chandigarh", "Rajasthan": "Jaipur", "Sikkim": "Gangtok",
    "Tamil Nadu": "Chennai", "Telangana": "Hyderabad", "Tripura": "Agartala",
    "Uttar Pradesh": "Lucknow", "Uttarakhand": "Dehradun", "West Bengal": "Kolkata"}
print("CAPITALS OF INDIAN STATES\n")
print("\n".join(f"{state} : {capital}" for state, capital in states_capitals.items()))
>program using STRING datatype
states_capitals = """CAPITALS OF INDIAN STATES
telangana : delhi
andhrapradesh : amaravathi
gujarath : gandhinagar"""
print(states_capitals)
> program using LIST datatype
>states_capitals = ["telangana : delhi", "gujarath : gandhinagar", "andhrapradesh : amaravathi"]
print("CAPITALS OF INDIAN STATES\n")
print("\n".join(states_capitals))
>using TUPLE
states_capitals = (
    ("telangana", "delhi"), ("gujarath", "gandhinagar"), ("andhrapradesh", "amaravathi")
    )
print("CAPITALS OF INDIAN STATES\n")
for state, capital in states_capitals:
    print(f"{state} : {capital}")
>OPRERATORS
>operator is a special symbol which performs operations on different values and variables allowing you to manipulate data by performing mathematical calculations, comparisons, assignments, and logical checks within your code; essentially, they are used to carry out actions on data like addition, subtraction
>PROGRAM 
a = 10
b = 20
print("the value of", a, " + ", 20, "is: ", a + b )
print("the value of", a, " - ", 20, "is: ", a - b )
print("the value of", a, " * ", 20, "is: ", a * b )
print("the value of", a, " / ", 20, "is: ", a / b )
print("the value of", a, " % ", 20, "is: ", a % b )
print("the value of", a, " ** ", 20, "is: ", a ** b )
print("the value of", a, " // ", 20, "is: ", a // b )
>CODE USING CONDITIONAL STATEMENTS
>PROGRAM
num1 = float(input("eneter first number: "))
operator = input("enter operatior (+, -, *, /): ")
num2 = float(input("enter second number: "))

if operator == '+':
    print(f"Result: {num1 + num2}")
elif operator == '-':
    print(f"Result: {num1} - {num2}")
elif operator == '*':
    print(f"Result: {num1} * {num2}")
elif operator == '/':
    if num2 != 0:
        print(f"Result: {num1} / {num2}")
    else:
        print("Error! Division by zero.")
else:
        print("invalid operator!")
>advantage: The primary advantage of operators in programming is that they allow developers to perform complex calculations and manipulations on data using concise, readable expressions, making code more efficient and easier to write by providing a simple way to execute various operations like arithmetic, logical, and comparison checks within a program
>disadvantage: Operators make code shorter but can also make it confusing if used too much in one line. Python follows rules for which operators run first, which can lead to unexpected results. This makes debugging harder, especially for beginners. Using parentheses helps clarify expressions and improves readability.
>TYPE CASTING
>Conversion of one datatype to another data type is called type casting
>two types
>explicit
>implicit
>EXPLICIT: conversion of one data type to other datatype via human or developer intervension with the requirement of python inbuilt funtions int(), float(), dict(), bool()etc
>EXAMPLE
>string = "7"
number = 20
string_number = int(string)
sum= number + string_number
print("sum of both numbers is: ", sum)
>a = "3"
b = "10"
print(int(a) + int(b))
>IMPLICIT: python datatypes donot have samelevel. there are higher order datatypes and lower order datatypes while performing operations on variables with datatypes lowerorder variable datatyoes converted to higher order variable datatypes in python. According to the level one datatype converted to other datatype by python interpreter itself.
>EXAMPLE
>a = 1.9
b = 8
print(a + b)
>OUTPUT
>9.9
>CODE
>nums = [2, 7, 11, 15]  # The list of numbers
target = 9  # The target sum we want to achieve

# Dictionary to store the value and its index
num_to_index = {}  # This will help us find numbers quickly

# Iterate through the array
for i, num in enumerate(nums):  # 'i' is the index, 'num' is the value at that index
    complement = target - num  # The 'complement' is the number we need to find
    if complement in num_to_index:  # Check if this 'complement' is already in our dictionary
        print([num_to_index[complement], i])  # Output the indices of the complement and the current number
        break  # Stop the loop since we found the answer
    num_to_index[num] = i  # Add the current number and its index to the dictionary
output
0 1
>CODE
a = input("enetr your name :")
print("my name is :",a)
x = input("enter first number :")
y = input("enter second number :")
print(x + y)
print(int(x) + int(y))
>OUTPUT
>CODE
>FACTORS OF 2
>limit = 100
for i in range(1, limit + 1):#range function in python generate sequence of numbers starting from frst argument to second argument
    if i % 2 == 0:
     print(i)
>EVEN NUMBERS
>a = int(input("enter a value x :"))
if a % 2 == 0:
    print("even")
else:
    print("not even")
>AREA OF THE CIRCLE
>r = 5
pi = 3.14
a = pi*r*r
print("area of the circle is :",a)














