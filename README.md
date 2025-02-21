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
Exception: Exceptions are types of errors that occur when the program is being executed and change the normal flow of the ptogram
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














