# interviewquestions
1. What is Python?
Python is a high-level, interpreted, interactive, and object-oriented scripting language. It uses English keywords frequently. Whereas, other languages use punctuation, Python has fewer syntactic constructions.
Python is designed to be highly readable and compatible with different platforms such as Mac, Windows, Linux, Raspberry Pi, etc.

2. Python is an interpreted language. Explain.
An interpreted language is any programming language that executes its statements line by line. Programs written in Python run directly from the source code, with no intermediary compilation step.

3. What is the difference between lists and tuples?
Lists	                                                                                          Tuples
Lists are mutable, i.e., they can be edited                                                   	Tuples are immutable (they are lists that cannot be edited)
Lists are usually slower than tuples	                                                          Tuples are faster than lists
Lists consume a lot of memory                                                                  	Tuples consume less memory when compared to lists
Lists are less reliable in terms of errors as unexpected changes are more likely to occur     	Tuples are more reliable as it is hard for any unexpected change to occur
Lists consist of many built-in functions.                                                     	Tuples do not consist of any built-in functions.
Syntax:                                                                                         Syntax:
list_1 = [10, ‘Intellipaat’, 20]                                                                tup_1 = (10, ‘Intellipaat’ , 20)

4. What are Python Modules?
Files containing Python codes are referred to as Python Modules. This code can either be classes, functions, or variables and saves the programmer time by providing the predefined functionalities when needed. It is a file with “.py” extension containing an executable code.
Commonly used built modules are listed below:
os
sys
data time
math
random
JSON

5. Explain Inheritance in Python with an example?
As Python follows an object-oriented programming paradigm, classes in Python have the ability to inherit the properties of another class. This process is known as inheritance. Inheritance provides the code reusability feature. The class that is being inherited is called a superclass or the parent class, and the class that inherits the superclass is called a derived or child class. The following types of inheritance are supported in Python:
Single inheritance: When a class inherits only one superclass
Multiple inheritance: When a class inherits multiple superclasses
Multilevel inheritance: When a class inherits a superclass, and then another class inherits this derived class forming a ‘parent, child, and grandchild’ class structure
Hierarchical inheritance: When one superclass is inherited by multiple derived classes

6. What is a dictionary in Python?
Python dictionary is one of the supported data types in Python. It is an unordered collection of elements. The elements in dictionaries are stored as key-value pairs. Dictionaries are indexed by keys.

For example, below we have a dictionary named ‘dict’. It contains two keys, Country and Capital, along with their corresponding values, India and New Delhi.

Syntax:

dict={‘Country’:’India’,’Capital’:’New Delhi’, }
Output: Country: India, Capital: New Delhi

7. What are functions in Python?
A function is a block of code which is executed only when a call is made to the function. def keyword is used to define a particular function as shown below:

def function():
print("Hi, Welcome to Intellipaat")
function(); # call to the function
Output:
Hi, Welcome to Intellipaat

8. What is __init__ in Python?
Equivalent to constructors in OOP terminology, __init__ is a reserved method in Python classes. The __init__ method is called automatically whenever a new object is initiated. This method allocates memory to the new object as soon as it is created. This method can also be used to initialize variables.

Syntax

(for defining the __init__ method):
class Human:
# init method or constructor
def __init__(self, age):
self.age = age
# Sample Method
def say(self):
print('Hello, my age is', self.age)
h= Human(22)
h.say()
Output:

Hello, my age is 22

9. What are the common built-in data types in Python?
Python supports the below-mentioned built-in data types:

Immutable data types:
Number
String
Tuple
Mutable data types:
List
Dictionary
set

10. What are local variables and global variables in Python?
Local variable: Any variable declared inside a function is known as Local variable and it’s accessibility remains inside that function only.

Global Variable: Any variable declared outside the function is known as Global variable and it can be easily accessible by any function present throughout the program.

g=4   #global variable
def func_multiply():
l=5       #local variable
m=g*l
return m
func_multiply()
Output: 20
If you try to access the  local variable outside the multiply function then you will end up with getting an error.

11. What is type conversion in Python?
Python provides you with a much-needed functionality of converting one form of data type into the needed one and this is known as type conversion.

Type Conversion is classified into types:

1.Implicit Type Conversion: In this form of Type conversion python interpreter helps in automatically converting the data type into another data type without any User involvement.

2.Explicit Type Conversion: In this  form of Type conversion the data  type inn changed into a required type by the user.
Various Functions of explicit conversion are show below:
int() –  function converts any data type into integer.
float() –   function converts any data type into float.
ord() – function returns an integer representing the Unicode character
hex() –  function converts integers to hexadecimal strings.
oct() –   function converts integer to octal strings.
tuple() – function convert to a tuple.
set() – function returns the type after converting to set.
list() – function converts any data type to a list type.
dict() – function is used to convert a tuple of order (key,value) into a dictionary.
str() –  function used to convert integer into a string.
complex(real,imag) – function used to convert real numbers to complex(real,imag) numbers.

12. Is indentation required in Python?
Indentation in Python is compulsory and is part of its syntax.

All programming languages have some way of defining the scope and extent of the block of codes. In Python, it is indentation. Indentation provides better readability to the code, which is probably why Python has made it compulsory.

13. What are Python packages?
A Python package refers to the collection of different sub-packages and modules based on the similarities of the function.

14. Explain split(), sub(), subn() methods of “re” module in Python?
These methods belong to the Python RegEx or ‘re’ module and are used to modify strings.

split(): This method is used to split a given string into a list.
sub(): This method is used to find a substring where a regex pattern matches, and then it replaces the matched substring with a different string.
subn(): This method is similar to the sub() method, but it returns the new string, along with the number of replacements.

15. What is a map function in Python?
The map() function in Python has two parameters, function and iterable. The map() function takes a function as an argument and then applies that function to all the elements of an iterable, passed to it as another argument. It returns an object list of results.

For example:
def calculateSq(n):
return n*n
numbers = (2, 3, 4, 5)
result = map( calculateSq, numbers)
print(result)

16. What are the generators in python?
Generator refers to the function that returns an iterable set of items.

17. What are python iterators?
These are the certain objects that are easily traversed and iterated when needed.

18. Do we need to declare variables with data types in Python?
No. Python is a dynamically typed language, I.E., Python Interpreter automatically identifies the data type of a variable based on the type of value assigned to the variable.

19. What are Dict and List comprehensions?
Python comprehensions are like decorators, that help to build altered and filtered lists, dictionaries, or sets from a given list, dictionary, or set. Comprehension saves a lot of time and code that might be considerably more complex and time-consuming.

Comprehensions are beneficial in the following scenarios:

Performing mathematical operations on the entire list
Performing conditional filtering operations on the entire list
Combining multiple lists into one
Flattening a multi-dimensional list
For example:

my_list = [2, 3, 5, 7, 11]
squared_list = [x**2 for x in my_list]    # list comprehension
# output => [4 , 9 , 25 , 49 , 121]

squared_dict = {x:x**2 for x in my_list}    # dict comprehension
# output => {11: 121, 2: 4 , 3: 9 , 5: 25 , 7: 49}

20. How do you write comments in python?
Python Comments are the statement used by the programmer to increase the readability of the code. With the help of #, you can define the single comment and the other way to do commenting is to use the docstrings(strings enclosed within triple quotes).
For example:

#Comments in Python 
print("Comments in Python ")






