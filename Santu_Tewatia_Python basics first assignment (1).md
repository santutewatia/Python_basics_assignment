```python
                           Python basics first assignment

Ques 1 explain the key features of Python that make its a popular choice for programming.

Ques 2  Describe the role of predefined keywords in Python and provide examples of how they ae used in a
programs

Ques 3 Compare and contrast mutable and immutable objects in Python with examples

Ques 4 Discuss the different types of operators in Python and provide examples of how they are used.

Ques 5 explain the concept of type casting in Python with examples.

Ques 6  How do conditional statements work in Python ? Illustrate with examples.

Ques 7 Describe the different types of loops in Python and their use cases with examples

```


```python
#Ques.1

#explain the key features of python that make its popular choices for programing


Python is popular for several reasons that make it easy and powerful to use:


1 Easy to Read and Write: Python's code looks like simple English, making it easier to understand and write, even for beginners.

2 Versatile: You can use Python for many different things, like building websites, analyzing data, creating games, and automating tasks. It’s a "do-it-all" language.

3 Huge Library of Tools: Python comes with a lot of pre-made tools and libraries that help you do things quickly, like handling data or creating visualizations. You don’t have to start from scratch.

4 Strong Community Support: There are lots of people who use Python, which means there are many resources, tutorials, and forums where you can get help.

5 Perfect for Data Science and AI: Python has become the go-to language for data science and artificial intelligence because it has powerful libraries that make these complex tasks easier.    

```


```python
# Ques.2

Describe the role of predefined keywords in Python and provide examples of how they are used in a
program.


Predefined keywords in Python, also known as reserved words, are integral to the language's syntax and cannot be used as identifiers, such as variable names or function names. These keywords have predefined meanings that enable the Python interpreter to understand the structure and behavior of a program.

Key Roles of Predefined Keywords in Python
1 Control Flow:  Keywords such as if, else, elif, for, while, break, continue, and pass control the flow of execution in a program.

2 Data Types and Values:  Keywords like True, False, and None represent specific constant values and are used in logical and comparison operations.

3 Function and Class Definitions:  Keywords like def, return, yield, lambda, and class define functions, generate values, create lambda expressions, and define classes, respectively.

4 Exception Handling:  Keywords such as try, except, finally, raise, assert, and with handle exceptions and ensure proper resource management.

5 Logical and Membership Operations:  Keywords like and, or, not, is, in, as, and from perform logical operations and define relationships between objects.

Examples of Using Keywords in Python Programs

Here are examples illustrating how these keywords are typically used:


```


```python
#1 Control Flow with if, else, and elif:

number = 7

if number > 0:
    print("The number is positive.")
elif number == 0:
    print("The number is zero.")
else:
    print("The number is negative.")
    
    
#Explanation: The keywords if, elif, and else are used to execute code blocks based on specific conditions
```


```python
#2 Looping with for and while:

# Using a `for` loop to iterate over a range of numbers
for i in range(3):
    print(i)

# Using a `while` loop to repeat an action until a condition is met
count = 0
while count < 3:
    print(count)
    count += 1
    
# Explanation: for is used for iterating over a sequence, while while is used for looping as long as a condition is true.
```

    0
    1
    2
    0
    1
    2
    


```python
# 3Defining Functions with def and Returning Values with return:

def multiply(a, b):
    return a * b

result = multiply(2, 3)
print(result)  # Output: 6

# Explanation: def is used to define a function, and return is used to output a value from the function.
```

    6
    


```python
#4 Exception Handling with try, except, and finally:
try:
    user_input = int(input("Enter a number: "))
    print(f"You entered: {user_input}")
except ValueError:
    print("Invalid input! Please enter a valid number.")
finally:
    print("Execution finished.")
    
# Explanation: try is used to attempt code that may cause an error, except handles the error if it occurs, and finally executes regardless of whether an error occurred.
```

    Enter a number: 12
    You entered: 12
    Execution finished.
    


```python
# 5 Using Boolean Values with True and False:
is_active = True
if is_active:
    print("The system is active.")
else:
    print("The system is not active.")

#     Explanation: True and False are used as Boolean values to control program logic
```

    The system is active.
    


```python
#6 Class Definition with class and Object Deletion with del:
class Dog:
    def __init__(self, name):
        self.name = name

    def bark(self):
        print(f"{self.name} says Woof!")

my_dog = Dog("Buddy")
my_dog.bark()  # Output: Buddy says Woof!

del my_dog  # Deletes the object `my_dog`

# Explanation: class is used to define a class, and del is used to delete an object.
```

    Buddy says Woof!
    


```python
# Using with for Resource Management:
with open("example.txt", "w") as file:
    file.write("Hello, World!")
# Explanation: with ensures proper acquisition and release of resources, like opening and closing files.
```


```python
# Ques 3

 Compare and contrast mutable and immutable objects in Python with examples

Mutable Objects

Mutable objects can be changed after they are created. You can modify their content, add new items, or remove items.
```


```python
# Examples of Mutable Objects:
#1 Lists: You can change, add, or remove elements.
my_list = [1, 2, 3]
my_list[0] = 10  # Change an element
print(my_list)  # Output: [10, 2, 3]
my_list.append(4)  # Add an element
print(my_list)  # Output: [10, 2, 3, 4]

```

    [10, 2, 3]
    [10, 2, 3, 4]
    


```python
#2 Dictionaries: You can change values or add/remove key-value pairs
my_dict = {"a": 1, "b": 2}
my_dict["a"] = 10  # Change a value
print(my_dict)  # Output: {'a': 10, 'b': 2}
my_dict["c"] = 3  # Add a new key-value pair
print(my_dict)  # Output: {'a': 10, 'b': 2, 'c': 3}

```

    {'a': 10, 'b': 2}
    {'a': 10, 'b': 2, 'c': 3}
    


```python
Immutable Objects

Immutable objects cannot be changed after they are created. If you want to change an immutable object, you have to create a new one.

```


```python
# Examples of Immutable Objects:

# 1 Strings: You can't change a string directly.
my_string = "hello"
new_string = my_string.upper()  # Creates a new string
print(new_string)  # Output: "HELLO"
print(my_string)  # Output: "hello" (original remains unchanged)

```

    HELLO
    hello
    


```python
#2 Tuples: Once created, the elements in a tuple cannot be modified
my_tuple = (1, 2, 3)
# my_tuple[0] = 10  # This would raise an error because tuples are immutable
print(my_tuple)  # Output: (1, 2, 3)


```

    (1, 2, 3)
    


```python
Key Differences

Mutable Objects: You can change them (like lists and dictionaries).
Immutable Objects: You cannot change them (like strings and tuples).
    
Summary:

Use mutable objects when you need to modify data, such as changing elements in a list.
Use immutable objects when you want to ensure that data does not change, like keeping a string or a tuple the same.
```


```python
# Ques 4 

 Discuss the different types of operators in Python and provide examples of how they are used.

 In Python, operators are special symbols that perform operations on values or variables. Here’s a simple guide to different types of operators and examples of how they are used:

 1. Arithmetic Operators

 These operators perform mathematical operations
```


```python
# Addition (+): Adds two values.
a = 5
b = 3
result = a + b
print(result)  # Output: 8

```

    8
    


```python
# Subtraction (-): Subtracts one value from another.
result = a - b
print(result)  # Output: 2

```

    2
    


```python
# Multiplication (*): Multiplies two values.
result = a * b
print(result)  # Output: 15

```

    15
    


```python
# Division (/): Divides one value by another (returns a float).
result = a / b
print(result)  # Output: 1.6666666666666667

```

    1.6666666666666667
    


```python
# Floor Division (//): Divides and returns the integer part of the result.
result = a // b
print(result)  # Output: 1

```

    1
    


```python
# Modulus (%): Returns the remainder of a division.
result = a % b
print(result)  # Output: 2

```

    2
    


```python
# Exponentiation (**): Raises one value to the power of another.
result = a ** b
print(result)  # Output: 125

```

    125
    


```python
 2. Comparison Operators
# These operators compare two values and return True or False.
```


```python
# Equal to (==): Checks if two values are equal.
print(a == b)  # Output: False

```

    False
    


```python
# Not equal to (!=): Checks if two values are not equal.
print(a != b)  # Output: True

```

    True
    


```python
# Greater than (>): Checks if one value is greater than another.
print(a > b)   # Output: True

```

    True
    


```python
# Less than (<): Checks if one value is less than another.
print(a < b)   # Output: False

```

    False
    


```python
# Greater than or equal to (>=): Checks if one value is greater than or equal to another.
print(a >= b)  # Output: True

```

    True
    


```python
# Less than or equal to (<=): Checks if one value is less than or equal to another.
print(a <= b)  # Output: False

```

    False
    


```python
3.Logical Operators
# These operators are used to combine conditional statements.
```


```python
# And (and): Returns True if both conditions are true.
print(a > 2 and b < 5)  # Output: True

```

    True
    


```python
# Or (or): Returns True if at least one condition is true.
print(a > 2 or b > 5)  # Output: True

```

    True
    


```python
# Not (not): Returns True if the condition is false.
print(not (a > 2))  # Output: False

```

    False
    


```python
4. Assignment Operators
# These operators are used to assign values to variables.
```


```python
# Assignment (=): Assigns a value to a variable.
x = 10

```


```python
# Add and Assign (+=): Adds a value to a variable and assigns the result.
x += 5
print(x)  # Output: 15

```

    15
    


```python
# Subtract and Assign (-=): Subtracts a value from a variable and assigns the result.
x -= 3
print(x)  # Output: 12

```

    12
    


```python
# Multiply and Assign (*=): Multiplies a variable by a value and assigns the result.
x *= 2
print(x)  # Output: 24

```

    24
    


```python
# Divide and Assign (/=): Divides a variable by a value and assigns the result.
x /= 4
print(x)  # Output: 6.0

```

    6.0
    


```python
5. Bitwise Operators
# These operators perform bit-level operations.
```


```python
# AND (&): Performs bitwise AND.
a = 5  # 0101 in binary
b = 3  # 0011 in binary
result = a & b
print(result)  # Output: 1 (0001 in binary)

```

    1
    


```python
# OR (|): Performs bitwise OR.
result = a | b
print(result)  # Output: 7 (0111 in binary)

```

    7
    


```python
# XOR (^): Performs bitwise XOR.
result = a ^ b
print(result)  # Output: 6 (0110 in binary)

```

    6
    


```python
# NOT (~): Performs bitwise NOT (inverts bits).
result = ~a
print(result)  # Output: -6 (inverts bits of 0101)

```

    -6
    


```python
# Left Shift (<<): Shifts bits to the left.
result = a << 1
print(result)  # Output: 10 (1010 in binary)

```

    10
    


```python
# Right Shift (>>): Shifts bits to the right.
result = a >> 1
print(result)  # Output: 2 (0010 in binary)

```

    2
    


```python
6. Identity Operators
# These operators compare the memory locations of two objects.
```


```python
# Is (is): Checks if two variables point to the same object.
x = [1, 2, 3]
y = x
print(x is y)  # Output: True

```

    True
    


```python
# Is Not (is not): Checks if two variables point to different objects.
z = [1, 2, 3]
print(x is not z)  # Output: True

```

    True
    


```python
7. Membership Operators
# These operators check if a value is in a sequence.
```


```python
# In (in): Checks if a value is present in a sequence.
list1 = [1, 2, 3]
print(2 in list1)  # Output: True

```

    True
    


```python
# Not In (not in): Checks if a value is not present in a sequence.
print(4 not in list1)  # Output: True

```

    True
    


```python
Summary:
    
Arithmetic Operators: Perform math operations.
Comparison Operators: Compare values.
Logical Operators: Combine conditions.
Assignment Operators: Assign values to variables.
Bitwise Operators: Perform operations on bits.
Identity Operators: Check if two objects are the same.
Membership Operators: Check if a value is in a sequence.
```


```python
# Ques 5

Explain the concept of type casting in Python with examples.

# Type casting in Python refers to the process of converting a variable from one data type to another.
#This is useful when you need to perform operations that require specific types or when you want to 
#ensure that data is handled correctly.
```


```python
# Basic Types and Type Casting

# Here are some common types and examples of how to cast between them:

# Casting to Integer (int)

# From Float to Integer: Converts a floating-point number to an integer. The decimal part is discarded.

num = 10.5
num_int = int(num)
print(num_int)  # Output: 10

```

    10
    


```python
# From String to Integer: Converts a string containing digits to an integer.
num_str = "123"
num_int = int(num_str)
print(num_int)  # Output: 123

```

    123
    


```python
#2 Casting to Float (float)

# From Integer to Float: Converts an integer to a floating-point number.
num = 10
num_float = float(num)
print(num_float)  # Output: 10.0

```

    10.0
    


```python
# From String to Float: Converts a string containing a decimal number to a float
num_str = "12.34"
num_float = float(num_str)
print(num_float)  # Output: 12.34

```

    12.34
    


```python
# 3 Casting to String (str)

# From Integer to String: Converts an integer to a string.
num = 100
num_str = str(num)
print(num_str)  # Output: "100"



```

    100
    


```python
# From Float to String: Converts a float to a string.
num = 10.5
num_str = str(num)
print(num_str)  # Output: "10.5"

```

    10.5
    


```python
# Casting to Boolean (bool)

# From Integer to Boolean: Converts an integer to a boolean. Any non-zero integer becomes True, while 0 becomes False.

num = 1
boolean_val = bool(num)
print(boolean_val)  # Output: True

num = 0
boolean_val = bool(num)
print(boolean_val)  # Output: False

```

    True
    False
    


```python
# From String to Boolean: Converts a string to a boolean. Non-empty strings become True, while an empty string becomes False

str_val = "Hello"
boolean_val = bool(str_val)
print(boolean_val)  # Output: True

str_val = ""
boolean_val = bool(str_val)
print(boolean_val)  # Output: False

```

    True
    False
    


```python
Summary

Type casting in Python is a crucial concept for converting data between types to ensure proper handling 
and manipulation. It involves both implicit conversions by Python and explicit conversions using
functions like int(), float(), str(), and bool(). Understanding type casting helps prevent errors
and enhances code versatility.

```


```python
# Ques 6

How do conditional statements work in Python? Illustate with exaples.

Conditional statements in Python allow you to execute different blocks of code based on certain
conditions. These statements use the if, elif, and else keywords to control the flow of the program
depending on whether specific conditions evaluate to True or False.

Key Components of Conditional Statements:

```


```python
# 1 if Statement:

# The if statement checks a condition. If the condition is True, the code block under the if statement
# is executed.

age = 18
if age >= 18:
    print("You are eligible to vote.")
# Output: "You are eligible to vote."

```

    You are eligible to vote.
    


```python
# 2 elif Statement:

# The elif (short for "else if") statement checks another condition if the previous if statement’s 
# condition was False. You can have multiple elif statements.
number = 0
if number > 0:
    print("Positive number")
elif number == 0:
    print("Zero")
# Output: "Zero"

```

    Zero
    


```python
#3 else Statement:

# The else statement runs a code block if none of the preceding if or elif conditions are True.
score = 45
if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
else:
    print("Grade: F")
# Output: "Grade: F"

```

    Grade: F
    


```python
# Ques 7

Describe the different types of loops in Python and their use cases with examples.

In Python, loops are used to execute a block of code repeatedly until a specified condition is met.
There are two primary types of loops in Python: the for loop and the while loop. Each has different 
use cases depending on the situation.
```


```python
1  for Loop

 The for loop in Python is used for iterating over a sequence (such as a list, tuple, string, or range).
 This type of loop is useful when you know in advance how many times you want to execute a statement
 or a block of statements.

Use Cases:

Iterating over a collection (like a list or a dictionary).
Executing a block of code a specific number of times using range().
Iterating through characters in a string.

```


```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
# Output:
# apple
# banana
# cherry                #exmaple

```

    apple
    banana
    cherry
    


```python
2. while Loop

The while loop continues to execute as long as the specified condition is True. This type of loop is 
useful when the number of iterations is not known beforehand, and the loop depends on some external
condition that changes during execution.

Use Cases:

Repeating an action until a condition changes.
Looping until user input meets a specific criterion.
Running tasks that need to keep checking for changes or updates.
```


```python
count = 0
while count < 5:
    print(count)
    count += 1
# Output:
# 0
# 1
# 2
# 3
# 4

```

    0
    1
    2
    3
    4
    


```python
3. Nested Loops

Both for and while loops can be nested inside each other. Nested loops are useful for iterating over 
multidimensional structures, such as lists of lists or grids.

```


```python
# Nested for Loop:
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
for row in matrix:
    for number in row:
        print(number, end=" ")
    print()
# Output:
# 1 2 3 
# 4 5 6 
# 7 8 9

```

    1 2 3 
    4 5 6 
    7 8 9 
    


```python
# while Loop with for Loop:
i = 1
while i <= 3:
    for j in range(1, 4):
        print(i, j)                       
    i += 1
# Output:
# 1 1
# 1 2
# 1 3
# 2 1
# 2 2
# 2 3
# 3 1
# 3 2
# 3 3

```

    1 1
    1 2
    1 3
    2 1
    2 2
    2 3
    3 1
    3 2
    3 3
    


```python
Summary

for Loop: Used for iterating over a sequence or a specific range of numbers. Best when the number
of iterations is known.

while Loop: Runs as long as a condition is True. Ideal when the number of iterations is not known
or depends on dynamic conditions.

Nested Loops: Allow iteration over complex data structures or performing more complicated logic
with multiple loops.
```


```python

```
