
# TABLE OF CONTENT
1. [BASICS](#brief-introduction-to-python)
    - [Imtroduction](#brief-introduction-to-python)
    - [Variable](#variable-naming-conventions-in-python)
    - [Comment](#comments-in-python)
    - [Datatypes](#data-types-in-python)
    - [String](#strings-in-python)
    - [Number](#numbers-and-math-in-python)

2. [CONTROL](#control-flow-and-exception-handling-in-python)
    - [ifs](#if-statement)
    - [elif](#elif-statement)
    - [try & except](#try-and-except-clauses)
    - [Common error](#common-exceptions-errors-in-python)

3. [DATA STRUCTURE](#data-structure)
    - [Tuple](#tuples-in-python)
    - [List](#lists-in-python)
    - [Set](#sets-in-python)
    - [Dictionary](#python-dictionaries)

4. [LOOPING](#range-function-for-loop-and-while-loop-in-python)
    - [for](#for-loop)
    - [while](#while-loop)
    - [control in loop](#common-loop-control-statements)

5. [REGULAR EXPRESSION](#regular-expressions-re-for-string-manipulayion)
    - [RE chars](#common-special-characters)
    - [Special sequence](#special-sequences)
    - [re functions](#main-functions)
    - [re flags](#common-flags)

6. [FUNCTION](#functions-in-python)
    - [def](#defining-a-function)
    - [return](#the-return-statement)
    - [Sope](#variable-scope)
    - [Parameters](#function-with-parameters)
    - [Order](#order-of-arguments)
    - [Docstring](#docstrings-in-functions)
    - [lambda](#lambda-functions)
    - [Best practices](#best-practices-with-functions)
    - [Creating module](#creating-your-own-python-module)

7. [Numpy into](#very-breif-intro-to-numpy)
    - [Intro](#very-breif-intro-to-numpy)
    - [Crating array](#creating-arrays)
    - [Slicing](#slicing)
    - [Shaping](#common-data-shaping-funtions-in-numpy)
    - [Math & Stats Funcs](#common-arithmetic-and-statistical-funtions-in-numpy)

8. [PANDAS](#introduction-to-pandas)
    - [Data creation](#pandas-data-structures)
    - [Data Loading](#data-loading-in-pandas)
    - [Exporting](#exporting-your-data-in-pandas)


# Brief Introduction to Python
Python is a general-purpose programming language. It is known for its simplicity and readability, making it one of the most popular programming languages today. Python was created by **Guido van Rossum** and was first released in 1991.
## Key Features:
1. It's open-source
2. Extensive library support for tasks like data analysis, machine learning, web development etc...
3. Its syntax is simple and resembles everyday English.
4. It has large active community that provides extensive resources and support.
5. Works on Windows, macOS, Linux, and more.

# Running Python Code
You can run Python code in different ways:

1. **Interactive Mode**:
   - Use a terminal or command prompt to type Python commands directly.
   - Example: Type `python` in the terminal and then type `print("Hello")`.

2. **Using an IDE**:
   - Use Integrated Development Environments (IDEs) like VS Code, PyCharm,  Jupyter Notebook etc...

3. **Online Platforms**:
   - Platforms like Google Colab and Replit allow you to run Python code in your browser.




# Simplicity of Python Syntax
Python is known for its clean and readable syntax, making it beginner-friendly and efficient for coding. To highlight this simplicity, let’s compare the famous "Hello, World!" program in Python with a few other programming languages.


### Comparison
We'll look at how we can print "Hello, World!" to the screen in the following programing language so that you can appreciate the simplicity of python language and not run away as we proceed!!!:
1. Python
2. C
3. Java
4. JavaScript
5. C++

**1. In python:**

```py
print("Hello World!")
```

---
**2. In C:**

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}

```
---

**3. In Java:**
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
---
**4. In javascript:**
```javascript
console.log("Hello, World!");
```
---
**5. c++:**
```c++
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```
---

# Functions in Python
Think of it as some special keyword designed to perform certain operation on objects. Python has a lot of built-in functions like print(), int(), sum(),
max(), min(), all(), any(), sorted(), reversed(), help() etc...

# Variable Naming Conventions in Python

A **variable** is a name that refers to a value stored in memory. Proper naming conventions make code easier to read and maintain.


### Key Points About Variables:
1. Variables are created when you assign a value to a name using `=`.
2. Python is **dynamically typed**, meaning you don't need to declare the type of a variable.
3. Variable names are **case-sensitive**. In fact, Python is generally **case-sensitive** unlike excel and SQL
   - `myVar` and `myvar` are treated as two different variables.

# Naming Conventions: Snake Case vs. Camel Case

### 1. Snake Case
 All lowercase with words separated by underscores (`_`).


**Example**:
```python
my_variable = 10
user_age = 25

```


### 2. Camel Case
tarts with lowercase and combined with words starting in uppercase.

**Example**:
```python
myVariable = 10
userAge = 25
```

# Rules for Naming Variables in Python

1. **Start with a Letter or Underscore (`_`)**:
   alid: `my_var`, `_hidden`.
   nvalid: `1st_var` (cannot start with a digit).

2. **Use Letters, Digits, and Underscores (`_`) Only**:
   Valid: `var1`, `some_var`.
   valid: `my-v` (hyphen is not allowed).

3. **Avoid Python Keywords**:
    Invalid: `if = 10`, `while = 5` (Python keywords cannot be used as variable names).

4. **No Spaces**:
    Invalid: `my var = 5` (use underscores instead: `my_var = 5`).
5. **NOTE:** 
   Interestingly, Pythone can allow you to use function name as a variable  name, but the trade- there is that you will not be able to use that function again except you claer it off Python memory by restarting the kenel or deleting it using `del` keyword



**I want you to define the following variable and run the code:**
```python
x = 10  
my_var = "Python"  
1st_var = 20  
if = "hello"  
print = 85
```

# Comments in Python

Comments are used to explain code and make it more readable. Comennts are indicated by starting with `#`. You use it to temporarily freeze your code too.


**Example**
```py
a = 6 # Assigning 6 to a
# multiplying a by 2
a * 2
```
# Data Types in Python

Data types define the type of value a variable holds. Python is a dynamicallyped language, meaning the data type is determined automatically when you assign a value to a variable. Data types are important in the sense that they define what operations can be performed on the data.



# Types

## 1. Numeric Types
**`int`**: Whole numbers (e.g., `1`, `42`, `-
**`float`**: Numbers with decimal points (e.g., `3.14`, `-5`).

## 2. Sequence Types
**`str`**: Strings, or sequences of characters (e.g., `"hello"`, `'world'`).
*`list`**: Ordered, mutable collections (e.g., `[1, 2, 3]`).
**`tuple`**: Ordered, immutable collections (e.g., `(1, 2, 3)`) etc....




## 3. Set Types
*`set`**: Unordered collections of unique elements (e.g., `{1, 2, 3}`).
`frozenset`**: Immutable version of a set.



## 4. Mapping Type
**`dict`**: Key-lue pairs (e.g., `{"name": "Alice", "age": 25}`).



## 5. Boolean Type
**`bool`**: Represents `True` or `False`.





# How to Check Data Types

Python provides the `type()` function to check the data type of a variable.


# Strings in Python
A string is a sequence of characters enclosed in quotes. Strings are one of the most commonly used data types in Python.

## Characteristics of Strings
1. Strings can be enclosed in single quotes (`'`), double quotes (`"`), or triple quotes (`'''` or `"""`).
2. Strings are **immutable**, meaning their content cannot be changed after creation.
3. Strings are ordered, allowing you to access specific characters using indexing.

## Examples of Strings:
`'Hello'`
`"World"`
`'''Python is awesome'''`

# Accessing Characters in Strings
Python strings are **indexed** and support both positive and negative indexing.

## Positive Indexing:
Starts from 0.
 Example: In `"Python"`, `P` is at index `0`, `y` is at index `1`, and so on.

## Negative Indexing:
 Starts from 1.
 Example: In `"Python"`, `n` is at index `1`, `o` is at `-2`, and so on.


# String Slicing
Slicing allows you to extract a subset of a string. The syntax is:  

string[start:end:step]

- **start**: The starting index (inclusive). Defaults to `0`.
- **end**: The ending index (exclusive). Defaults to the length of the string.
- **step**: The interval between indices. Defaults to `1`.

## String Concatenation and Replication
- Two or more strings can be joined together using `+` For instane, "boy" + "girl" = "boygirl"
- Strings can be repeated in two or more times using `*` For instane, "boy" * 2 = "boyboy"
## Membership check
You can check if a substring is in a string or not.
- Something like this:
    - "a" in "Farming"
    - "c" not in "Machine"
# Some String Methods
Python provides several built-in methods to work with strings. Methods are functions applied to objects

## Commonly Used Methods:
1. **`lower()`**: Converts all characters to lowercase.
2. **`upper()`**: Converts all characters to uppercase.
3. **`strip([string])`**: Removes leading and trailing whitespace or other strings.
4. **`replace(old, new)`**: Replaces all occurrences of `old` with `new`.
5. **`find(substring)`**: Returns the index of the first occurrence of a substring and return `-1` if none is found.
6. **`index(substring)`**: Behaves like finde but throws error if none is found.
7. **`capitalize()`**: Converts the first characters to uppercase.
8. **`title()`**: Converts the first characters of each word to uppercase.
9. **`startswith(substring)` and `endswith(substring)`**: Check if the string starts or ends with the specified substring.


Explore More!



## STRING IMMUTABILITY
Strings in Python are immutable, meaning their content cannot be changed after they are created. You can only change them by updating them.

## Handling New Lines and Tab in String
`\` is a special character in python. It's use for escaping and it functions as special character in strings as well  
'\n' -------> newline  
'\t' -------> tab


# Raw String
use r'string' to indicte that you are interested in all the content in a string

# Tripple Quotation String
Tripple quotation string preserve all the caracters in a string including white spaces



## NUMBERS AND MATH IN PYTHON

## Float and Integer Data Types
Integers (int) are whole numbers, which can be positive, negative, or zero. For example, 10, -7, and 0 are integers.  
Floating-point numbers (float) represent numbers with a fractional part, such as 3.14, -2.0, or 0.5.  You can determine the type of a number using the type() function  

## Conversion Between Float, Integer, and String
Python allows datatype conversion between floats, integers, and strings using built-in functions:  

- int(): Converts a value to an integer by truncating the fractional part. For instance, int(4.99) will return 4.  

- float(): Converts a value to a floating-point number. For example, float(3) will return 3.0.  

- str(): Converts a value to a string. For instance, str(42) will return '42'.

Note that you can cast from string too to integer or float as long as their string representation is valid. You can't convert a string version of float to integer but you can convert string version of integer to float


## Arithmetic Operations and Expressions


Use `+` for addition, `-` for subtraction, `*` for multiplication, and `/` for division.
Use `//` for floor division (which reduce the result to an integer i.e. withouth the fractional part) and `%` for the remainder (`modulus division`).
Use `**` for exponentiation (raising to a power).

Python follows the order of operations when evaluating arithmetic expressions. This order is summarized by the acronym PEMDAS:  

**P** stands for parentheses: operations inside parentheses are performed first.  
**E** stands for exponentiation: powers are evaluated next.  
**MD** stands for multiplication and division: these are evaluated from left to right.  
**AS** stands for addition and subtraction: these are evaluated last, also from left to right.  


## Math Functions

Python provides useful built-in functions and the math module for performing advanced mathematical calculations:

- The math.sqrt() function calculates the square root of a number.

- The math.ceil() function rounds a number up to the nearest integer.

- The math.floor() function rounds a number down to the nearest integer.

- The math.factorial() function calculates the factorial of a number.
etc...


Python also has general-purpose functions for numbers:

- The round() function rounds a number to the specified number of decimal places. For instance, round(3.14159, 2) will return 3.14.  
- The abs() function returns the absolute value of a number. For example, abs(-5) will return 5.    


`Note that you have to import math module before you can use its function or you can import a specific function from math module.`   

## String Interpolation (f-Strings)

String interpolation allows you to embed variables and expressions directly within strings. There are many ways to format strings in Python but the most modern and esiest way  is by using f-strings (formatted string literals).

An f-string is created by prefixing the string with f or F.

Place variables or expressions inside curly braces {} to interpolate them.

You can also format numbers within f-strings (e.g., controlling decimal places, coma thousand seperator, zero padding, percentages) etc....


## The eval() Function in Python

The eval() function in Python is a built-in function that evaluates a string as a Python expression. It can execute any valid Python code embedded in the string and return the result of the evaluation.

Be careful with it while using user input though!!!


## User Input

You can take input from the user using the input() function. The input is always returned as a string, so you need to convert it to an integer or float if you want to perform numeric operations.  


# Control Flow and Exception Handling in Python

## Conditional Operators in Python
Conditional operators in Python are used to compare two values or expressions, returning a Boolean value: either True or False. They form the foundation of decision-making in programming.  
1. `==` (Equal to): This operator checks if two values are equal. If they are, it returns True; otherwise, it returns False.
 
2. `!=` (Not equal to): This operator checks if two values are not equal. If they are not equal, it returns True; otherwise, it returns False.
 
3. `<` (Less than):
This operator checks if the value on the left is less than the value on the right.
  
4. `>` (Greater than): This operator checks if the value on the left is greater than the value on the right.

5. `<=` (Less than or equal to): This operator checks if the value on the left is less than or equal to the value on the right.


6. `>=` (Greater than or equal to): This operator checks if the value on the left is greater than or equal to the value on the right.

These operators are important for writing `if` statements, loops, and other decision-making code in Python. Each comparison evaluates to True or False, which determines the flow of the program.


## Logical Operators (and, or, not) with Boolean Comparison
Logical operators allow you to combine multiple conditions.
How Logical Operators Work:

- `and`: Returns True if all conditions are true.

- `or`: Returns True if at least one condition is true.

- `not`: Negates a Boolean value (returns the opposite).


## Order of Logical Operators
Logical operators follow this order of precedence:

1. not
2. and
3. or


## if Statement
The if statement allows your program to execute a block of code only when a specific condition is true. Once you declare if statement, you must end it with colon `:`, then the next line of code must be indented. 
Something like this:  


if condition:  
&nbsp; &nbsp; &nbsp; &nbsp;Code to execute if condition is true

***`Take note of the indentation after if condition`***

## else Statement
The else statement defines a block of code to execute when the if condition is false.  

Something like this:  

if condition:  
&nbsp; &nbsp; &nbsp; &nbsp;Code if condition is true  
else:  
&nbsp; &nbsp; &nbsp; &nbsp;Code if condition is false  

## elif Statement

The elif (short for "else if") statement checks additional conditions when the previous if or elif conditions are false.  

Something like this:  

if condition1:  
&nbsp; &nbsp; &nbsp; &nbsp;Code if condition1 is true  
elif condition2:  
&nbsp; &nbsp; &nbsp; &nbsp;Code if condition2 is true  
else:  
&nbsp; &nbsp; &nbsp; &nbsp;Code if none of the conditions are true  

## Nested if Statements

Nested if statements are if conditions inside another if. They are used to check multiple levels of conditions.
Something like this:  

if condition1:  
&nbsp; &nbsp; &nbsp; &nbsp;if condition2:  
&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;Code if both conditions are true  

# Exception Handling

An exception is an error that occurs during the execution of a program, disrupting its normal flow. Unlike syntax errors, exceptions occur while the program is running.


## Common Exceptions (Errors) in Python

Here are some common exceptions you might encounter:

1. ZeroDivisionError: Raised when you divide by zero.

2. ValueError: Raised when a function gets an invalid argument.


3. TypeError: Raised when an operation is performed on incompatible types.


4. IndexError: Raised when accessing an invalid index in a list.


## try and except Clauses

To beg python to pardon your exceptions error so that you code does not crash, you can use try and except clauses. The code inside the try block runs first. If an exception occurs, the code in the except block is executed.
Something like this structure (take note of the indent):  

`try`:  
&nbsp; &nbsp; &nbsp; &nbsp;Code that may raise an exception  
except ExceptionType:  
&nbsp; &nbsp; &nbsp; &nbsp;Code to handle the exception  

## Handling Multiple Exceptions

You can handle multiple exceptions using multiple except blocks.  

## Using else and finally with try

`else`: Runs if no exception occurs.  

`finally`: Always executes, whether an exception occurs or not.  


## Data Structure


## Tuples in Python

Tuples are one of Python's fundamental data structures, used to store collections of items. Tuples can contain elements of different data types (e.g., integers, strings, floats).

#### Creating Tuples

Tuple can be created by simply using parethesis.  
something like this:  
a = ()  

Confirm the datatype of a  


#### Single-Element Tuple  

You must include a trailing comma when creating a tuple with a single element; otherwise, it will be treated as a regular value.  

## Accessing Tuple Elements
Tuples are zero-indexed. You can access the element the same way you access that of a string. You can even access a range of elements using slicing:    

## Characteristics of Tuples

- Just like string, tuples cannot be modified after creation (e.g., no addition, deletion, or changing of elements). This immutability makes them faster and safer for fixed data.


- Elements in a tuple have a fixed order. You can access elements using their index.


- Tuples can contain duplicate elements.


- Tuples can store elements of different data types (e.g., numbers, strings, other tuples).

## Tuple Operations

Just like string, you can do some operation with tuple  like concatenation, replication, membership check

- concatenation
```py
b = (1,5,True,"meat")
c = ("fat","item7")
c+ b
```
- replication
```py
b = (1,5,True,"meat")
c = ("fat","item7")
c * 4
```
- membership check
```py
b = (1,5,True,"meat")
5 in b
```


## Tuple Methods
Tuples have only two built-in methods due to their immutability:  

count(): Counts the occurrences of an element.
```py
bb = ("rice","bread","yam","rice","egg")
bb.count("rice")
```

index(): Finds the index of the first occurrence of an element.

```py
bb = ("rice","bread","yam","rice","egg")
bb.index("rice")
```

## Unpacking the Elements of Tuples
You can assign the elements of tuple to a new variable by simply unpacking them individually or in groups

```py
cc = (2,7)
x,y = cc
print(x)
print(y)
tt = ("rice","bread","yam","rice","egg")
e,f,*j = tt
print(e)
print(f)
print(j)
*k,m,g = tt 
print(k,m,g)
```

## Lists in Python  
Lists are one of the most commonly used data structures in Python. They are mutable, ordered collections that can hold a variety of data types. In other words, A list is an ordered collection of items (also called elements) enclosed in square brackets [ ]

## Characteristics of Lists  
- The order of elements is preserved, and each element has an index starting from 0.


- Lists can be modified (e.g., add, remove, or change elements), that is, unlike string and tuple, lists are mutable
- Lists can store elements of different data types.
- Lists can contain duplicate elements.

## Accessing List Elements  

Apply the same principle from string and tuple!!!

## Modifying Lists
You can update elements of list in place through list methods or index address
```py
gg = ["rice","bread","yam","rice","egg"]
print(gg)
gg[0] = "beans"
print(gg)
gg[-2:] = ["ice cream"]
print(gg)
```


## List Operations  

Similar to that of string and tuple. You can concatenate, replicate and check for membership

## List Methods

| Method   | Description                                                                                                                                                                                                                                                                                                                                                                    |
|:---------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| append   | Append object to the end of the list.                                                                                                                                                                                                                                                                                                                                          
| clear    | Remove all items from list.                                                                                                                                                                                                                                                                                 
| copy     | Return a shallow copy of the list.                                                                                                                                                                                                                                                                                                                                             
| count    | Return number of occurrences of value.                                                                                                                                                                                                                                                                                                                                         
| extend   | Extend list by appending elements fiterable.                                                                                                                                                                                                                                                                                                                           
| index    | Return first index of value.  Raises ValueError if the value is not present.                                                                                                                                                                                                                                                                                                
| insert   | Insert object before index.                                                                                                                                                                                                                                                                                                                                                    |
| pop      | Remove and return item at index (default last).  Raises IndexError if list is empty or index is out of range.                                                                                                                                                                                                                                                                  
| remove   | Remove first occurrence of value.  Raises ValueError if the value is not present.                                                                                                                                                                                                                                                                                     
| reverse  | Reverse *IN PLACE*.                                                                                                                                                                                                                                                                                                                                                            |
| sort     | Sort the list in ascending order and return None.  The sort is in-place (i.e. the list itself is modified) and stable (i.e. the order of two equal elements is maintained).  If a key function is given, apply it once to each list item and sort them, ascending or descending, according to their function values.  The reverse flag can be set to sort in descending order. |

- append, insert, extend
```py
gg = ["rice","bread","yam","rice","egg"]
print(gg)
gg.append("Semo")
print(gg)
gg.insert(1,"vegetable")
print(gg)
hh = ["dodo","tea","eba"]
gg.append(hh)
gg.extend(hh)
print(gg)
```
- sort, reverse, pop, remove, clear
```py
gg = ["rice","bread","yam","rice","egg"]
# use this for copy to avoid unexpected behaviouer 
ui = gg[:]
print(ui)
gg.clear()
print(gg)
p = ui.pop()
print(p)
print(ui)
ui.remove("rice")
print(ui)
ui.reverse()
print(ui)
# In case you dont want to reverse the list in place
list(reversed(ui))

rsv = ["apple","Axe","pig","POT","mat"]
print(rsv)
# By default python prioritize capital letter 
# overwrite it by usuing key= str.lower in sort method 
# By default sorting is in ascending order 
# You can change it by using reverse=True in sort method 
rsv.sort(key=str.lower,reverse=True)
print(rsv)
```

## Sets in Python


Sets in Python are a type of collection that store unique, unordered, and mutable elements. They are commonly used when you need to eliminate duplicates or perform mathematical set operations like union, intersection, difference etc....


### Characteristics of Sets
The elements in a set do not have a defined order.

Sets automatically remove duplicate values.  
You can add or remove elements from a set, but the set itself is unordered.  
Sets can store elements of different data types.  
Since sets are unordered, elements cannot be accessed using an index.

## Set Operations and Methods
Sets support mathematical operations like union, intersection, difference, etc symmetric difference.


| Method                      | Description                                                                                                                                                     |
|:----------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| add                         | Add an element to a set.  This has no effect if the element is already present.                                                                                 |
| clear                       | Remove all elements from this set.                                                                                                                              |
| copy                        | Return a shallow copy of a set.                                                                                                                                 |
| difference                  | Return a new set with elements in the set (let's say set A) that are not in the others ((let's say set B)). You can also use `-` operator **e.g (A - B)**.                                                             
| difference_update           | Update the set, removing elements found in others.                                                                                                              |
| discard                     | Remove an element from a set if it is a member.  Unlike set.remove(), the discard() method does not raise an exception when an element is missing from the set. |
| intersection                | Return a new set with elements common to the set and all others You can also use `&` operator **e.g (A & B)**.                                                                             
| intersection_update         | Update the set, keeping only elements found in it and all others.                                                                                               |
| isdisjoint                  | Return True if two sets have a null intersection.                                                                                                               |
| issubset                    | Report whether another set contains this set.                                                                                                                   |
| issuperset                  | Report whether this set contains another set.                                                                                                                   |
| pop                         | Remove and return an arbitrary set element.  Raises KeyError if the set is empty.                                                                               |
| remove                      | Remove an element from a set; it must be a member.  If the element is not a member, raise a KeyError.                                                           |
| symmetric_difference        | Return a new set with elements in either the set or other but not both You can also use `^` operator **e.g (A ^ B)**.                                                                                         
| symmetric_difference_update | Update the set, keeping only elements found in either set, but not in both.                                                                                     |
| union                       | Return a new set with elements from the set and all others You can also use `\|` operator **e.g (A \| B)**.                                                                    
| update                      | Update the set, adding elements from all others.                                                                                                                |




## Python Dictionaries
A dictionary in Python is a collection of key-value pairs. Each key in the dictionary is unique, and it is used to store and retrieve data efficiently. 


**Characteristics of Dictionaries** 


- Unordered: Dictionaries do not maintain the order of elements (prior to Python 3.7). However, from Python 3.7 onwards, dictionaries maintain insertion order. In other words, a dictionary is an unordered, mutable collection of key-value pairs enclosed in curly braces {}

- Mutable: You can add, remove, or modify key-value pairs.

- Unique Keys: No duplicate keys are allowed. If a key is repeated, the last value will overwrite the previous one.

- Efficient Lookup: Keys allow fast data retrieval.

### Accessing and Modifying Elements
Accessing Values  ------>   Use the key to retrieve the corresponding value. Just like we do in list, tuple and strings but this one, you make use of key as your index.

### Some Useful Dictionary Methods

| Method     | Description                                                                                                                                                                                                                                                                                             |
|:-----------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| clear      | Remove all items from the dict.                                                                                                                                                                                                                                                                         |
| copy       | Return a shallow copy of the dict.                                                                                                                                                                                                                                                                      |
| fromkeys   | Create a new dictionary with keys from iterable and values set to value.                                                                                                                                                                                                                                |
| get        | Return the value for key if key is in the dictionary, else default.                                                                                                                                                                                                                                     |
| items      | Return a set-like object providing a view on the dict's items.                                                                                                                                                                                                                                          |
| keys       | Return a set-like object providing a view on the dict's keys.                                                                                                                                                                                                                                           |
| pop        | D.pop(k[,d]) -> v, remove specified key and return the corresponding value.  If the key is not found, return the default if given; otherwise, raise a KeyError.                                                                                                                                         |
| popitem    | Remove and return a (key, value) pair as a 2-tuple.  Pairs are returned in LIFO (last-in, first-out) order. Raises KeyError if the dict is empty.                                                                                                                                                       |
| setdefault | Insert key with a value of default if key is not in the dictionary.  Return the value for key if key is in the dictionary, else default.                                                                                                                                                                |
| update     | D.update([E, ]**F) -> None.  Update D from mapping/iterable E and F. If E is present and has a .keys() method, then does:  for k in E.keys(): D[k] = E[k] If E is present and lacks a .keys() method, then does:  for k, v in E: D[k] = v In either case, this is followed by: for k in F:  D[k] = F[k] |
| values     | Return an object providing a view on the dict's values.                                                                                                                                                                                                                                                 |



**NOTE**
- `All these data structure can be converted from one to the othere using their class`


## Range Function, For Loop, and While Loop in Python
### range() Function  
The range() function generates a sequence of numbers. It’s often used in loops for iteration.

Syntax:  
```py
range(start, stop, step)  
```
- start (optional): The number to start the sequence from. Defaults to 0.  
- stop: The number at which the sequence ends (exclusive).  
- step (optional): The difference between each number in the sequence. Defaults to 1.  


``Note that range() does not generate a list or other python data structure we have covered by default; it produces a range object. Convert it to a list using list(range()) if needed.``

## For Loop
The for loop in Python is used to iterate over a sequence (e.g., list, tuple, string, or range).
## Nested For Loop
A for loop inside another for loop.

## While Loop
The while loop continues to execute as long as the condition is True.

TAKE NOTE OF THESE EXPRESSIONS IN PYTHON!!!

`x += 1` -------> x = x + 1 (that is, you increase variable x by 1)  
`x -= 1` -------> x = x - 1 (that is, you decrease variable x by 1)  
`x *= 1` -------> x = x * 1 (that is, you multiply variable x by 1)  
`x /= 1` -------> x = x / 1 (that is, you divide variable x by 1)...etc


#### Common Loop Control Statements
`break` ------->	Exits the loop prematurely.  
`continue` -------> Skips the current iteration and moves to the next.  
`pass` -------> Does nothing (used as a placeholder in the code block).




## Python Comprehensions  
Python comprehensions provide a concise and efficient way to create sequences like lists, dictionaries, and sets. They are often used as a shorter alternative to traditional loops for generating these structures.  


 ### List Comprehension
Syntax

[**expression** for **item** in **iterable** if **condition**]


**expression**: The operation or value to include in the list.  
**item**: Variable representing the element from the iterable.  
**iterable**: The data to loop through (e.g., list, range, etc.).  
**condition** (optional): A filter applied to items in the iterable.

## Dictionary Comprehension  
Just like list comprehension


Syntax

{key_expression: value_expression for item in iterable if condition}

## Set Comprehension

Syntax  
{expression for item in iterable if condition}

It is similar to the rest

## Generator Expressions
Syntax  
Similar to list comprehension but uses parentheses () instead of square brackets [].

Key Difference:


List comprehensions create the entire list in memory, while generator expressions generate items on demand (memory-efficient).

## Enumerate in Loops
The enumerate() function adds a counter to an iterable and returns it as an enumerate object, which can be used in loops.

Syntax  
enumerate(**iterable**, **start**=0)

**iterable**: The sequence to enumerate.
**start**: The starting value of the counter (default is 0).
## Python zip() Function  
The zip() function in Python is used to combine two or more iterables (e.g., lists, tuples, strings) into a single iterable of tuples. Each tuple contains one element from each of the input iterables, grouped together based on their corresponding positions.

### Characteristics of zip()
Creates an Iterator: The result of zip() is an iterator. To see the combined elements, you must convert it to a list, tuple, or another iterable.  
Stops at the Shortest Iterable: If the input iterables have different lengths, zip() stops when the shortest iterable is exhausted.

Syntax  
zip(iterable1, iterable2, ...)




## Regular Expressions (re) for String Manipulayion

* `re` provides pattern matching and text searching similar to Perl.
* Regular expressions are built from ordinary and special characters.
* Ordinary characters (e.g. `A`, `a`, `1`) simply match themselves.


### Common Special Characters

|      Symbol      | Meaning                                                       |                                             
| :--------------: | :------------------------------------------------------------ | 
|        `.`       | Matches any character except newline              
|       `[]`       | Matches any **one character inside brackets (e.g. `[a-z]`). |                                            
|      `[^ ]`      | Matches any character not inside brackets.                |                                            
|       `()`       | Groups pattern; can capture text for reuse.                   |
| `\|` | Acts as OR operator |                                    
                                      

### **Special Sequences**

| Sequence | Description                           |
| :------: | :------------------------------------ |
|   `\d`   | Any digit = `[0-9]`.                |
|   `\D`   | Any non-digit =  `[^0-9]`                 |
|   `\s`   | Any whitespace (`space, \t, \n`). |
|   `\S`   | Any non-whitespace.               |
|   `\w`   | Any alphanumeric or underscore = `[A-Za-z0-9_]`  |
|   `\W`   | Any non-word character = `[^A-Za-z0-9_]`           |
|   `\\`   | Literal backslash.                    |

### Quantifiers

|  Quantifier      |  Description                                                                     |
|:-----------------|:---------------------------------------------------------------------------------|
| `*`              | Matches 0 or more repetitions of previous RE (greedy                             |
| `+`              | Matches 1 or more repetitions (greedy).                                          |
| `?`              | Matches 0 or 1 of previous RE (greedy).                                          |
| `*?`, `+?`, `??` | Non-greedy versions.                                                             |
| `{m,n}`          | Matches between m and n repetitions.                                             |
| `{m,n}?`         | Non-greedy version of above.                                                     |

### Assertion

|      Symbol      | Meaning                                                       |                                             
| :--------------: | :------------------------------------------------------------ | 
|   `\A`   | Start of string only.                 |
|   `\Z`   | End of string only.                   |
|   `\b`   | Word boundary.                        |
|   `\B`   | Non-word boundary.                    |
|        `^`       | Matches the start of a string.                                |                           
|        `$`       | Matches the end of a string.                        
|     `(?:...)`    | Non-capturing group.                                          |                                      
|     `(?=...)`    | Positive lookahead (must follow).                             |                                         
|     `(?!...)`    | Negative lookahead (must not follow).                         |                                      
|    `(?<=...)`    | Positive lookbehind (must precede).                           |                                       
|    `(?<!...)`    | Negative lookbehind.                                          |


---

### **Main Functions**

| Function      | Description                                                  |
| :------------ | :----------------------------------------------------------- |
| `match()`     | Checks for a match at the beginning of a string.         |
| `fullmatch()` | Matches the entire string.                               |
| `search()`    | Finds the first occurrence anywhere in the string.       |
| `findall()`   | Returns all matches as a list.                           |
| `finditer()`  | Returns an iterator of Match objects.                    |
| `split()`     | Splits string by occurrences of pattern.                     |
| `sub()`       | Replaces pattern matches with new text.                      |
| `compile()`   | Compiles RE into a reusable pattern object.                  |


---

### **Common Flags**

|  Flag  | Name       | Description                                  |
| :----: | :--------- | :------------------------------------------- |
| `re.I` | IGNORECASE | Case-insensitive matching.                   |
| `re.S` | DOTALL     | `.` matches newline too.                     |
| `re.X` | VERBOSE    | Ignore spaces and comments in pattern.       |

Explore more in re module.....


run this code
```py
import re
print(re__doc__)
```

# Functions in Python

A function is a reusable block of code designed to perform a specific task. Functions allow us to organize code into smaller, manageable parts, making it more readable, reusable, and efficient.



## Types of Functions in Python:
1. **Built-in Functions**:
   - Predefined in Python (e.g., `print()`, `len()`, `sum()`).
2. **User-defined Functions**:
   - Created by the programmer using the `def` keyword.

   # Defining a Function

Use the `def` keyword to define a function. The basic syntax is:

```python
def function_name(parameters):
    # Function body
   
```
# The `return` Statement

The `return` statement is used to send a result back to the caller. Without it, the function returns `None`.

***Syntax***:
```python
def function_name(parameters):
    # Perform some operations
    return result
```
# Variable Scope

Scope determines where a variable can be accessed in your program. There are two types:

1. **Local Scope**:
   - Variables declared inside a function are accessible only within that function.

2. **Global Scope**:
   - Variables declared outside any function are accessible throughout the program.

# Function with Parameters

Functions can accept input values (parameters) to perform tasks dynamically. The values provided to the parameters are called **arguments**.


***Syntax***:
```python
def function_name(param1, param2):
    # Use parameters in the function
    return result
```
# Default Parameters

A function can have default parameter values. If no argument is provided for that parameter, the default value is used.


***Syntax***:
```python
def function_name(param1=value1, param2=value2):
    # Function body
```

# Arbitrary Positional Arguments (`*args`)

The `*args` parameter allows you to pass a variable number of positional arguments to a function. These arguments are collected into a tuple.


### **Syntax**:
```python
def function_name(*args):
   check type(args)
```
# Arbitrary Keyword Arguments (`**kwargs`)

The `**kwargs` parameter allows you to pass a variable number of keyword arguments to a function. These arguments are collected into a dictionary.


### ***Syntax***:
```python
def function_name(**kwargs):
    check type(kargs)

```
# Combining `*args` and `**kwargs`

You can use both `*args` and `**kwargs` in the same function. This allows you to handle an unknown number of positional and keyword arguments.


***Syntax***:
```python
def function_name(*args, **kwargs):
    # args is a tuple, kwargs is a dictionary
```
# Order of Function Arguments in Python

In Python, function arguments must follow a specific order when defining and calling a function.

### **Order of Arguments**:
1. **Positional Arguments**: Regular arguments passed in the correct order.
2. **Default Arguments**: Arguments with default values.
3. **Arbitrary Positional Arguments (`*args`)**: Collects extra positional arguments into a tuple.
4. **Keyword-only Arguments (`kw=`)**: Keyword **must** be declared. 
4. **Arbitrary Keyword Arguments (`**kwargs`)**: Collects extra keyword arguments into a dictionary.


***Syntax***:
```python
def function_name(positional, default=5, *args, **kwargs):
    # Function body
```

# Docstrings in Functions

A **docstring** (short for "documentation string") is a special kind of string that describes the purpose and behavior of a function, class, or module. It is written as the first statement inside the function and is enclosed in triple quotes (`'''` or `"""`).



### **Purpose of Docstrings**:
1. To explain what the function does.
2. To describe the parameters and return values.
3. To provide usage examples sometimes.

### Format of Docstrings

```py
def function_name(arguments):
"""
Description of what the function does.
Description of the arguments, if any.
Description of the return value(s), if any.
Description of errors raised, if any.
Optional extra notes or examples of usage.
"""
```
**Syntax**:
```python
def function_name(parameters):
    """
    A brief description of the function.

    Args:
        param1 (type): Description of param1.
        param2 (type): Description of param2.

    Returns:
        type: Description of the return value.
    """
    # Function body
```

### Google-style Docstrings

```py
def function(arg_1, arg_2=42):
"""Description of what the function does. 

Args: 
    arg_1 (str): Description of arg_1 that can break onto the next line if     needed. 
    arg_2 (int, optional): Write optional when an argument has a default value. 

Returns: 
    bool: Optional description of the return value Extra lines are not indented. 
    
Raises: 
    ValueError: Include any error types that the function intentionally raises. 

Notes: 
    More info you want to add.

```

### Numpydoc-style Docstrings
```py
def function(arg_1, arg_2=42):
"""
Description of what the function does.

Parameters
----------
arg_1 : expected type of arg_1
Description of arg_1.
arg_2 : int, optional
Write optional when an argument has a default value.
Default=42.

Returns
-------
The type of the return value
Can include a description of the return value.


    
Raises
---------
Include any error types that the function intentionally raises. 

Notes
----------
More info you want to add.

"""

```
# Lambda Functions

A **lambda function** is a small, anonymous function defined using the `lambda` keyword. It can have any number of arguments but only one expression.



***Syntax***:
```python
lambda arguments: expression
```
### ***Best Practices with Functions***:
1. Always follow the argument order: `positional` --->  `default` ---> `*args` ---> `**kwargs`.
2. Use meaningful names for `*args` and `**kwargs` when possible:
   - Example: `*numbers`, `**details`.
3. Avoid using too many arguments in a single function to maintain readability.
4. Add doc string a withnd annotation.

### Full example


Given the quadratic expression:![$ax^2 + bx + c = 0$](https://latex.codecogs.com/png.latex?x%5E2), and its corresponding quadratic formula:


 ![ $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$](https://latex.codecogs.com/png.latex?x%5E2)


 where:

 $a$ represents the coefficient of $x^2$, $b$ represents the coefficient of $x$, and $c$ represents the constant (the last term in the expression).

$ Discriminant (D) = b^2 - 4ac$


`Note that quadratic equation has no real solution if D < 0`

**Task:**

Write a python function that can solve quadratic equation

**Solution:**

```py

def qd_fun(a:float|int,
           b:float|int,
           c:float|int) -> str:
    
    """This function is designed to 
    solve quadratic equation
    
    Parameters
    -----------------------
        a: int, float

        coefficient of x squared

        b: int, float

        coefficient of x

        c: int, float

        the constant
        
    Returns
    ----------------
        str

        This function will retun the two values of x
        if the solution exists otherwise it will retun 
        `no solution`"""
    # representing discriminant
    D = b**2 - 4*a*c
    if D < 0:
        res = "No solution"
        return res
    else:
        import math
        implementing the quadratic formula
        x1 = (-b + math.sqrt(b**2 - 4*a*c))/(2*a)
        x2 = (-b - math.sqrt(b**2 - 4*a*c))/(2*a)
        res = f"x = {x1} or x = {x2}"
        return res

```

# Creating your own Python Module

A **module** is a file containing Python code, such as functions, variables, or classes, that can be reused in other scripts. Modules allow you to organize your code into separate files for better structure and reusabilit

### **Steps to Create a Module**:
1. Write your functions or variables in a `.py` file.
2. Save the file with a meaningful name (e.g., `my_module.py`).
3. Import the module into another script using the `import` statement.



### **Example**:
1. Create a file called `math_operations.py` with the following content:
```python
def add(a, b):
    """Adds two numbers."""
    return a + b

def subtract(a, b):
    """Subtracts the second number from the first."""
    return a - b
```
You then import it and start using it



# Very Breif Intro to NumPy

NumPy (Numerical Python) is a powerful Python library for numerical computing. It provides support for:
- Multi-dimensional arrays and matrices.
- Mathematical functions for operations on arrays etc....
- Alternative to Python List: NumPy Array
- Calculations over entire arrays
- Easy and Fast
- Perform element-wise operations without loops.
- Easily integrates with other libraries like pandas, matplotlib etc...


### **Installing NumPy**:
To install NumPy, use the following command:
```python
pip install numpy
```
# Creating NumPy Arrays

The core of NumPy is the `ndarray`, a multi-dimensional array object.


### **Creating Arrays**:
- **From a Python List**
```python
import numpy as np
array = np.array([1, 2, 3])

```
- **Using NumPy Functions**
    - np.zeros(shape): Creates an array of zeros.
    - np.ones(shape): Creates an array of ones.
    - np.arange(start, stop, step): Creates a range of numbers.
    - np.linspace(start, stop, num): Creates evenly spaced numbers....etc

**Note:** NumPy arrays: contain only one type etc...

Note that as we can have list of lists, we can have more than one dimensional array too.



# Indexing and Slicing in NumPy

You can access elements in a NumPy array using indexing and slicing.


### Indexing
- Access elements using their index (0-based).
- For multi-dimensional arrays, use `array[[level(in hiher dim]),row, column]`.

### Slicing
Use the syntax `start:stop:step` to slice an array.

**Example**
```py
arr2d = np.array([[3,4,6],[5,6,4],[7,84,7]])
print(arr2d[1,2])
print(arr2d[:,1])
print(arr2d[2,2])
print(arr2d[1:,1:])
```

### Common Data Shaping Funtions in Numpy

- reshape()
- flatten()
- transpose() ....etc

### Common Arithmetic and Statistical Funtions in Numpy

-  add(a, b)      
-  subtract(a, b) 
-  multiply(a, b) 
-  divide(a, b)   
-  mean()         
-  median()       
-  std()          
-  var()          
-  sum()          
-  min()          
-  max()          
-  cumsum()      
-  cumprod()...etc




# Introduction to Pandas

Pandas is a powerful and flexible Python library for data manipulation and analysis. It provides two main data structures: **Series** and **DataFrame**, which are built on top of NumPy arrays.

### **Key Features of Pandas**
- Provides Series and DataFrame for data manipulation.
- Works seamlessly with structured data from sources like CSV, Excel, SQL databases, and more.
- Provides tools for filtering, sorting, grouping, merging, and reshaping data.
- Easily integrates with other data science libraries like NumPy, Matplotlib etc...

### **Installing Pandas**
To install Pandas, run the following command:
```python
pip install pandas 
```
---
# Pandas Data Structures

Pandas provides two primary data structures for working with data:

## **1. Series**
- A one-dimensional labeled array capable of holding data of any type (integer, float, string, etc.).
- Similar to a column in a spreadsheet or a 1D NumPy array but with labels (indices).

### **Creating a Series**
- From list
```py
import pandas as pd
ls1 = ["Amala",True,2,34.65,"beans"]
ser1 = pd.Series(ls1)
display(ser1)
```
- From dictionary
```py
dict1 = {"A":"aja","B":'bata',1:"one",2:"two"}
ser2 = pd.Series(dict1)
display(ser2)
```
## **2. DataFrame**

A **DataFrame** is a two-dimensional, tabular data structure in Pandas. It consists of rows and columns, where:
- Rows are indexed (labeled with numbers by default).
- Columns have labels (names) and can store different data types.



### **Creating a DataFrame**
You can create a DataFrame from various data structures, such as:
- Python dictionaries
```py
import pandas as pd 
stud_info = {
    "name": ["Khadijat","Oluwadahunsi",
             "Halimat","Friday","Ayo"],
    "age":[9,7,12,5,10],
    "favourite food":["biscuit","eba",
                      "rice","Eba","Amala"]

}

df1 = pd.DataFrame(stud_info)
display(df1)
```
- Lists of lists
```py
l3 = [["Khadijat",9,"biscuit"],
      ["Oluwadahunsi",3,"eba"]]
df2 = pd.DataFrame(l3,columns=["name","age","food"])
display(df2)
```
- NumPy arrays
```py
num_1_100 = np.arange(1,101).reshape(20,5)
num_1_100
df3 = pd.DataFrame(num_1_100)
display(df3)
```
- Existing files (e.g., CSV, Excel) (a whole topic on its own)




## **Data Loading in Pandas**

### **1. CSV Files**

* Use the `read_csv()` function in pandas to read `.csv`, `.txt`, or `.tsv` files into a DataFrame.
* By default, pandas assumes that the data is **comma-delimited (`sep=","`)**.
* For other delimiters:

  * Use `sep="\t"` for tab-separated data.
  * Use `sep=";"` for semicolon-separated data.
  * Use any other string as needed, e.g. `sep="|"` for pipe-separated files.
* `header:` You can use the `header` argument to specify which row should be used as column headers.
- `skiprows:` skips specific rows at the start when reading a file. You can also pass a list of row indices to skip:
- `skipfooter:` skips a specified number of lines from the bottom of the file. It requires the `engine='python'` argument though
- `usecols:` selects specific columns to load.
- `nrows:` limits the number of rows read into the DataFrame. It's useful for previewing large datasets
-  `na_values: ` specifies additional strings to recognize as `NaN`.
-  `index_col:` sets a specific column (or multiple columns) as the index
- etc....explore more

```py
import pandas as pd 
game = pd.read_csv(
    r"C:\Users\Dell\Desktop\bt\vgchartz-2024.csv",
    # header=1,
    # skiprows=5,
    # skiprows=[4,8,11,56],
    # skipfooter=10,
    # engine="python",
    # nrows=5
    # na_values="PS3",
    index_col=["title"]


)
game 
```


### **2. Excel Files**

* Use the `read_excel()` function in pandas to read `.xls` or `.xlsx` files into a DataFrame.
* You must have **`openpyxl`** (for `.xlsx`) or **`xlrd`** (for older `.xls`) installed.
* Some important arguments include:

  * `sheet_name:` specify the sheet to load (name, index, or list of sheets).
  * `usecols:` load only specific columns.
  * `skiprows:` skip certain rows from the top.
  * `nrows:` limit the number of rows read.
  * `header:` set which row to use as column headers.
  * `index_col:` choose a column to be used as index.
  * `na_values:` specify custom missing value indicators.
* etc... explore more

```py
import pandas as pd 

gdp_per_cap = pd.read_excel(
    r"C:\Users\Dell\Desktop\bt\DOC-20250806-WA0007..xls",
    # skiprows=3,
    # sheet_name="Metadata - Countries",
    # sheet_name=2,
    # sheet_name=None,
    # usecols=
    
)
gdp_per_cap

fgcl = pd.read_excel(
    r"C:\Users\Dell\Desktop\bt\Workbooks\bt\FGCI.xlsx",
    header=1,
    usecols="c:d"
)
fgcl
```

### **3. Clipboard Data**

* Use the `read_clipboard()` function to read data copied to your clipboard*directly into a DataFrame.
* It’s useful for quickly importing tables from webpages, Excel, or other sources without saving them to a file.
* By default, pandas assumes tab-separated data (`sep='\t'`).
* You can specify other delimiters using the `sep` argument.



# **DATA LOADING (CONT'D)**
### **4. Loading data from mysql directly into pandas**
- step 1:
    + Install sqlalchemy
    + install pymysql
```py
! pip install sqlalchemy
! pip install pymysql
```
Importing engine creation class

```py
from sqlalchemy import create_engine 
```

### setting up your sql engine
- reqirements
    - **`username`** (we all used root, can you still remember?)
    - **`password`** (The password you created during sql class)


Let's hide our password by saving it environment variable
- Press window button + S
- Type edit environment variable
- Click on edit environment variable
- Under Environment variable, click new
- Enter any name you want (let it be a valid python variable name) in `variable name`
- Enter your sql password in `variable value`
- Press OK till end

### Use os module to bring the password into your notebook
- Use getenv function in os modele to fetch the password you saved in your environment variable (the arguement it takes is the variable name you used in `'edit environment variable'` in the step above). If it doesnt work restart your system.
- if you have "@" or any other special character in your password that may have conflict with sql create engine syntax, parse it with urlib.parse.quote 

```py
import os 
password = os.getenv("sql_psw")
# parsing pwd
from urllib.parse import quote
password = quote(password)
# seting up the engine
from sqlalchemy import create_engine
eng = create_engine(
    f"mysql+pymysql://root:{password}@localhost/today_class"
)
```


### Proceeding to Pandas
- Use pd.read_sql or pd.read_sql_query to fetch data from your mysql database

```py
import pandas as pd 
data = pd.read_sql(
    """

select * from
today_class.gns_exam_rec


""",con=eng
)
data
```

Explore more on other data file.....


## Exporting your data in pandas


* You can export your DataFrame to various file formats using Series and DataFrame method. Common ones include:

  * `to_csv()` --> exports to CSV file.
  * `to_exce l()` --> exports to Excel file
  * `to_clipboard()`--> copies the DataFrame to your clipboard.
  * `to_sql()` → writes the DataFrame to a **SQL database table**.
* Use arguments like `index=False` to avoid exporting the index and `na_rep='N/A'` to specify missing value representations.
* etc... explore more



