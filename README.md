Coding Journey
# abiodun


*VARIABLE and Data Types
Variable are use in storing information. They are created the moment a value or an ingredients is assoigned to it.
Python has no command for declaring a variable. Variables are used in storing data values.
 RULES OF VARIABLE
#A Variable name can start with a letter or underscore character and also alohanumeric character.
#Cannot start with a number.
#They are case sensitive.
#The reserved words(keywords) in Python cannot be used to name the variable in Python.

An Example of a Variable in Python is a representational name that serves as a pointer to an object. Once an object is assigned to a variable, it can be referred to by that name. In layman’s terms, we can say that Variable in Python is containers that store values.
i.e Var = "Wonderful"
print(Var)
The output will be Wonderful

Python Assign Values to Multiple Variables
Also, Python allows assigning a single value to several variables simultaneously with “=” operators.
For example:
a = b = c = 10

print(a)
print(b)
print(c)

The Python plus operator + provides a convenient way to add a value if it is a number and concatenate if it is a string. If a variable is already created it assigns the new value back to the same variable.
a = 10
b = 20
print(a+b)

a = "Greatfor"
b = "Great"
print(a+b)

Global and Local Python Variables
Local variables in Python are the ones that are defined and declared inside a function. We can not call this variable outside the function.
Global variables in Python are the ones that are defined and declared outside a function, and we need to use them inside a function.
# This function uses global variable s
def f():
    s = "Data epics"
    print(s)


f()


Python global is a keyword that allows a user to modify a variable outside of the current scope. It is used to create global variables from a non-global scope i.e inside a function. Global keyword is used inside a function only when we want to do assignments or when we want to change a variable. Global is not needed for printing and accessing.
Rules of global keyword
If a variable is assigned a value anywhere within the function’s body, it’s assumed to be local unless explicitly declared as global.
Variables that are only referenced inside a function are implicitly global.
We use a global in Python to use a global variable inside a function.
There is no need to use a global keyword in Python outside a function.
x = 15

def change():

    # using a global keyword
    global x

    # increment value of a by 5
    x = x + 5
    print("Value of x inside a function :", x)


change()
print("Value of x outside a function :", x)


The value stored in a variable can be changed during program execution.
A Variables in Python is only a name given to a memory location, all the operations done on the variable effects that memory location.

# numberic
var = 123
print("Numeric data : ", var)


# Boolean
print(type(True))
print(type(False))


# Creating a Dictionary
# with Integer Keys
Dict = {1: 'Geeks', 2: 'For', 3: 'Computer'}
print("\nDictionary with the use of Integer Keys: ")
print(Dict)

OUTPUT
Numeric data :  123
<class 'bool'>
<class 'bool'>

Set with the use of String:
{'r', 'G', 'e', 'k', 'o', 's', 'F'}

Dictionary with the use of Integer Keys:
{1: 'Geeks', 2: 'For', 3: 'Computer'

#DATA TYPES
Data types are the classification or categorization of data items. It represents the kind of value that tells what operations can be performed on a particular data. Since everything is an object in Python programming, data types are actually classes and variables are instances (object) of these classes. The following are the standard or built-in data types in Python:

Numeric
Sequence Type
Boolean
Set
Dictionary
Binary Types

To define the values <200b><200b>of various data types and check their data types we use the type() function. Consider the following examples.
# DataType Output: str
x = "Hello World"

# DataType Output: int
x = 50

# DataType Output: float
x = 60.5

# DataType Output: complex
x = 3j

# DataType Output: list
x = ["Pawpaw", "for", "Fruits"]

# DataType Output: tuple
x = ("Blood", "for", Sweat ")

# DataType Output: range
x = range(10)

# DataType Output: dict
x = {"name": "Suraj", "age": 24}

# DataType Output: set
x = {"python", "for", "coding"}

# DataType Output: frozenset
x = frozenset({"God is faithful", "for", "me"})

# DataType Output: bool
x = True

# DataType Output: bytes
x = b"Geeks"

# DataType Output: bytearray
x = bytearray(4)

# DataType Output: memoryview
x = memoryview(bytes(6))

# DataType Output: NoneType
x = None

The numeric data type in Python represents the data that has a numeric value. A numeric value can be an integer, a floating number, or even a complex number. These values are defined as Python int, Python float, and Python complex classes in Python.

Integers – This value is represented by int class. It contains positive or negative whole numbers (without fractions or decimals). In Python, there is no limit to how long an integer value can be.
Float – This value is represented by the float class. It is a real number with a floating-point representation. It is specified by a decimal point. Optionally, the character e or E followed by a positive or negative integer may be appended to specify scientific notation.
Complex Numbers – Complex number is represented by a complex class. It is specified as (real part) + (imaginary part)j. For example – 2+3j
Note – type() function is used to determine the type of data type.
# Python program to
# demonstrate numeric value

a = 5
print("Type of a: ", type(a))

b = 5.0
print("\nType of b: ", type(b))

c = 2 + 4j
print("\nType of c: ", type(c))

Output:

Type of a:  <class 'int'>

Type of b:  <class 'float'>

Type of c:  <class 'complex'>O[O]


Sequence Data Type in Python
The sequence Data Type in Python is the ordered collection of similar or different data types. Sequences allow storing of multiple values in an organized and efficient fashion. There are several sequence types in Python –
Python String
Python List
Python Tuple
String Data Type
Strings in Python are arrays of bytes representing Unicode characters. A string is a collection of one or more characters put in a single quote, double-quote, or triple-quote. In python there is no character data type, a character is a string of length one. It is represented by str class.

Creating String
Strings in Python can be created using single quotes or double quotes or even triple quotes.


# Python Program for
# Creation of String

# Creating a String
# with single Quotes
String1 = 'Welcome to the Geeks World'
print("String with the use of Single Quotes: ")
print(String1)

# Creating a String
# with double Quotes
String1 = "I'm a Geek"
print("\nString with the use of Double Quotes: ")
print(String1)
print(type(String1))

# Creating a String
# with triple Quotes
String1 = '''I'm a Geek and I live in a world of "Geeks"'''
print("\nString with the use of Triple Quotes: ")
print(String1)
print(type(String1))

# Creating String with triple
# Quotes allows multiple lines
String1 = '''Geeks
            For
            Life'''
print("\nCreating a multiline String: ")
print(String1)

String with the use of Single Quotes:
Welcome to the Geeks World

String with the use of Double Quotes:
I'm a Grateful
<class 'str'>

String with the use of Triple Quotes:
I'm a divine being and I live in a world of "Divines"
<class 'str'>

Creating a multiline String:
Geeks
            For
            Life
BOB
List Data Type
Lists are just like arrays, declared in other languages which is an ordered collection of data. It is very flexible as the items in a list do not need to be of the same type.

Creating List

Lists in Python can be created by just placing the sequence inside the square brackets[].


# Creating a List
List = []
print("Initial blank List: ")
print(List)

# Creating a List with
# the use of a String
List = ['GeeksForGeeks']
print("\nList with the use of String: ")
print(List)

# Creating a List with
# the use of multiple values
List = ["Geeks", "For", "Geeks"]
print("\nList containing multiple values: ")
print(List[0])
print(List[2])

# Creating a Multi-Dimensional List
# (By Nesting a list inside a List)
List = [['Geeks', 'For'], ['Geeks']]
print("\nMulti-Dimensional List: ")
print(List)


Tuple Data Type
Just like a list, a tuple is also an ordered collection of Python objects. The only difference between a tuple and a list is that tuples are immutable i.e. tuples cannot be modified after it is created. It is represented by a tuple class.
Creating a Tuple
In Python, tuples are created by placing a sequence of values separated by a ‘comma’ with or without the use of parentheses for grouping the data sequence. Tuples can contain any number of elements and of any datatype (like strings, integers, lists, etc.). Note: Tuples can also be created with a single element, but it is a bit tricky. Having one element in the parentheses is not sufficient, there must be a trailing ‘comma’ to make it a tuple.

# Creating an empty tuple
Tuple1 = ()
print("Initial empty Tuple: ")
print(Tuple1)

# Creating a Tuple with
# the use of Strings
Tuple1 = ('Geeks', 'For')
print("\nTuple with the use of String: ")
print(Tuple1)

# Creating a Tuple with
# the use of list
list1 = [1, 2, 4, 5, 6]
print("\nTuple using List: ")
print(tuple(list1))

# Creating a Tuple with the
# use of built-in function
Tuple1 = tuple('Geeks')
print("\nTuple with the use of function: ")
print(Tuple1)

# Creating a Tuple
# with nested tuples
Tuple1 = (0, 1, 2, 3)
Tuple2 = ('python', 'geek')
Tuple3 = (Tuple1, Tuple2)
print("\nTuple with nested tuples: ")
print(Tuple3)

Boolean Data Type in Python
Data type with one of the two built-in values, True or False. Boolean objects that are equal to True are truthy (true), and those equal to False are falsy (false). But non-Boolean objects can be evaluated in a Boolean context as well and determined to be true or false. It is denoted by the class bool.

Note – True and False with capital ‘T’ and ‘F’ are valid booleans otherwise python will throw an error.
# Python program to
# demonstrate boolean type

print(type(True))
print(type(False))


Create a Dictionary
In Python, a Dictionary can be created by placing a sequence of elements within curly {} braces, separated by ‘comma’. Values in a dictionary can be of any datatype and can be duplicated, whereas keys can’t be repeated and must be immutable. The dictionary can also be created by the built-in function dict(). An empty dictionary can be created by just placing it in curly braces{}. Note – Dictionary keys are case sensitive, the same name but different cases of Key will be treated distinctly.
# Creating an empty Dictionary
Dict = {}
print("Empty Dictionary: ")
print(Dict)

# Creating a Dictionary
# with Integer Keys
Dict = {1: 'Geeks', 2: 'For', 3: 'Geeks'}
print("\nDictionary with the use of Integer Keys: ")
print(Dict)

# Creating a Dictionary
# with Mixed keys
Dict = {'Name': 'Good', 1: [1, 2, 3, 4]}
print("\nDictionary with the use of Mixed Keys: ")
print(Dict)

# Creating a Dictionary
# with dict() method
Dict = dict({1: 'Geeks', 2: 'For', 3: 'Geeks'})
print("\nDictionary with the use of dict(): ")
print(Dict)

# Creating a Dictionary
# with each item as a Pair
Dict = dict([(1, 'Great'), (2, 'For')])
print("\nDictionary with each item as a pair: ")
print(Dict)
#*
