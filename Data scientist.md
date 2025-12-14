# Python
Python is one of the most popular programming languages. It’s simple to use, packed with features and supported by a wide range of libraries and frameworks. Its clean syntax makes it beginner-friendly.

A high-level language, used in data science, automation, AI, web development and more.
Known for its readability, which means code is easier to write, understand and maintain.
Backed by strong library support, we don’t have to build everything from scratch.

```Code`
# Python Program to Print Hello World!

print("Hello World!")


# Why Learn Python?
1️⃣ Easy to Learn, Easy to Read

Python syntax is simple and close to English

Less code, more work

Best language for beginners

print("Hello, World")

2️⃣ Widely Used in Many Fields

Python is used in almost every tech domain:

Field	Usage
Web Development	Django, Flask
Data Science	Pandas, NumPy
AI & ML	TensorFlow, PyTorch
Automation	Scripts, bots
Cyber Security	Testing tools
Game Dev	Pygame
3️⃣ High Demand & High Salary

Python developers are highly demanded

Used by companies like Google, Netflix, Amazon

Many high-paying jobs require Python

4️⃣ Perfect for Students & Exams (BCA / MCA)

Easy to write in exams

Clean syntax → fewer mistakes

Supports OOP, File Handling, Exception Handling

5️⃣ Best Language for AI, ML & Data Science

Almost all ML algorithms are implemented in Python

Libraries:

NumPy

Pandas

Scikit-learn

TensorFlow

6️⃣ Saves Time & Increases Productivity

Write programs faster than C/C++/Java

Great for prototyping

Focus on logic, not syntax

7️⃣ Huge Community & Learning Resources

Millions of tutorials, videos, and forums


Easy to get help

Continuous updates

8️⃣ Cross-Platform Language

Runs on Windows, Linux, Mac

Write once, run anywhere

9️⃣ Supports OOP + Functional Programming
class Student:
    def __init__(self, name):
        self.name = name

🔟 Strong Foundation for Other Languages

Concepts learned in Python help with:

Java

C++

JavaScript


input and Output (I/O) in Python allow a program to take data from the user and display results on the screen.

📥 Input in Python

Python uses the input() function to take input from the user.

🔹 Syntax
variable = input("Message to user")

🔹 Example
name = input("Enter your name: ")
print(name)


📌 Important:
input() always returns data as string (str).

🔄 Type Conversion (Very Important)

To perform calculations, convert input to required data type.

🔹 Integer Input
age = int(input("Enter age: "))
print(age)

🔹 Float Input
price = float(input("Enter price: "))
print(price)

📤 Output in Python

Python uses the print() function to display output.

🔹 Syntax
print(value)

🖨️ Different Ways to Print Output
1️⃣ Print Text
print("Hello Python")

2️⃣ Print Variables
x = 10
print(x)

3️⃣ Print Multiple Values
a = 5
b = 10
print(a, b)

4️⃣ Using sep (Separator)
print(1, 2, 3, sep="-")


Output:

1-2-3

5️⃣ Using end
print("Hello", end=" ")
print("World")


Output:

Hello World

🔗 String Formatting (Best Practice)
1️⃣ Using Comma (Simple)
name = "Amit"
age = 20
print("Name:", name, "Age:", age)

2️⃣ Using format()
print("Name: {} Age: {}".format(name, age))

3️⃣ Using f-string (Recommended)
print(f"Name: {name}, Age: {age}")


✔ Clean
✔ Fast
✔ Modern Python

🧪 Example Program (Input + Output)
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

sum = a + b
print("Sum =", sum)

⚠️ Common Mistakes

❌ Forgetting type conversion
❌ Using input() directly in calculations
❌ Wrong indentation

📌 Exam-Ready Short Answer

Input in Python is taken using the input() function, which returns a string. Output is displayed using the print() function. Type conversion functions like int() and float() are used to convert input into required data types.
ML algorithms

# Variables in Python — Deep & Clear Explanation

A variable in Python is a name that refers to a value stored in memory.
Python variables are dynamic, meaning you don’t need to declare their type in advance.

📌 What is a Variable?

A variable is a container used to store data values during program execution.

🔹 Example
x = 10
name = "Amit"
pi = 3.14


Here:

x stores an integer

name stores a string

pi stores a float

🧠 How Python Variables Work (Internals – Important)

In Python:

Variables do not store values directly

They store references (addresses) to objects in memory

a = 10
b = a


Both a and b point to the same object (10) in memory.

You can check this:

print(id(a))
print(id(b))

🔁 Dynamic Typing in Python

Python is dynamically typed.

x = 10      # int
x = "Hi"    # now string
x = 3.5     # now float


✔ No error
✔ Type changes at runtime

🧱 Variable Naming Rules (Very Important for Exams)
✅ Valid Rules

Must start with a letter (a–z, A–Z) or underscore (_)

Can contain letters, numbers, underscore

Case-sensitive (age ≠ Age)

Cannot use keywords

❌ Invalid Names
1name     ❌
my-name   ❌
class     ❌ (keyword)

✅ Valid Names
name
_age
total_marks
studentName

🔤 Types of Variables in Python
1️⃣ Local Variable

Defined inside a function.

def show():
    x = 10
    print(x)

show()


Accessible only inside the function

2️⃣ Global Variable

Defined outside a function.

x = 20

def show():
    print(x)

show()


Accessible everywhere

3️⃣ Using global Keyword

To modify global variable inside function:

x = 10

def update():
    global x
    x = 20

update()
print(x)

📦 Multiple Assignment
🔹 Same Value
a = b = c = 5

🔹 Multiple Values
x, y, z = 1, 2, 3

🔹 Swap Variables (Python Feature)
a, b = b, a


(No temporary variable needed!)

🧮 Variable Types (Based on Data Stored)
Type	Example
int	x = 10
float	x = 3.14
str	x = "Python"
bool	x = True
list	x = [1,2,3]
tuple	x = (1,2)
dict	x = {"a":1}

Check type:

print(type(x))

🔐 Mutable vs Immutable Variables (Very Important)
🔹 Immutable (Cannot change)

int

float

str

tuple

x = 10
x = x + 1   # new object created

🔹 Mutable (Can change)

list

dict

set

lst = [1, 2]
lst.append(3)


Same object modified ✔

🧪 Example Program
name = input("Enter name: ")
age = int(input("Enter age: "))

print(f"Name: {name}")
print(f"Age: {age}")

⚠️ Common Mistakes

❌ Using keywords as variables
❌ Forgetting type conversion
❌ Confusing = with ==
❌ Assuming variable stores value directly

📌 Exam-Ready Definition

A variable in Python is a name that refers to a memory location where data is stored. Python supports dynamic typing, so a variable can store different types of data during execution

# Operators in Python — Detailed & Clear Explanation

An operator in Python is a symbol or keyword used to perform operations on variables and values.

📌 What is an Operator?

Operators are special symbols that perform operations like addition, comparison, assignment, and logical decisions.

🔹 Example
x = 10
y = 5
print(x + y)

🧠 Types of Operators in Python

Python has 7 main types of operators:

Arithmetic Operators

Assignment Operators

Comparison (Relational) Operators

Logical Operators

Bitwise Operators

Membership Operators

Identity Operators

1️⃣ Arithmetic Operators

Used for mathematical calculations.

Operator	Meaning	Example	Result
+	Addition	10 + 5	15
-	Subtraction	10 - 5	5
*	Multiplication	10 * 5	50
/	Division	10 / 4	2.5
//	Floor Division	10 // 4	2
%	Modulus	10 % 4	2
**	Exponent	2 ** 3	8
🔹 Example
a = 10
b = 3
print(a + b, a - b, a * b)

2️⃣ Assignment Operators

Used to assign values to variables.

Operator	Example	Equivalent
=	x = 5	x = 5
+=	x += 3	x = x + 3
-=	x -= 2	x = x - 2
*=	x *= 2	x = x * 2
/=	x /= 2	x = x / 2
%=	x %= 2	x = x % 2
🔹 Example
x = 10
x += 5
print(x)

3️⃣ Comparison (Relational) Operators

Used to compare two values.
Result is always True or False.

Operator	Meaning	Example
==	Equal to	5 == 5
!=	Not equal	5 != 3
>	Greater than	5 > 3
<	Less than	5 < 3
>=	Greater or equal	5 >= 5
<=	Less or equal	5 <= 6
🔹 Example
a = 10
b = 5
print(a > b)

4️⃣ Logical Operators

Used to combine conditions.

Operator	Meaning	Example
and	True if both true	a > 5 and b < 10
or	True if any one true	a > 5 or b > 10
not	Reverse result	not(a > 5)
🔹 Example
age = 20
print(age > 18 and age < 30)

5️⃣ Bitwise Operators

Operate on binary values.

Operator	Name	Example
&	AND	5 & 3
`	`	OR
^	XOR	5 ^ 3
~	NOT	~5
<<	Left shift	5 << 1
>>	Right shift	5 >> 1
🔹 Example
print(5 & 3)   # 101 & 011 = 001

6️⃣ Membership Operators

Used to check presence in a sequence.

Operator	Meaning	Example
in	Present	'a' in 'apple'
not in	Not present	'x' not in 'apple'
🔹 Example
fruits = ["apple", "banana"]
print("apple" in fruits)

7️⃣ Identity Operators

Check if two variables refer to the same object in memory.

Operator	Meaning	Example
is	Same object	a is b
is not	Different object	a is not b
🔹 Example
a = [1, 2]
b = a
print(a is b)

🔐 Operator Precedence (Important)

Order of execution:

()

**

* / // %

+ -

Comparison

Logical (not, and, or)

🔹 Example
print(10 + 2 * 3)   # Output: 16

⚠️ Common Mistakes

❌ Confusing = with ==
❌ Using is instead of ==
❌ Wrong operator precedence
❌ Forgetting parentheses

📌 Exam-Ready Definition

Operators in Python are symbols used to perform operations on operands. Python supports arithmetic, assignment, comparison, logical, bitwise, membership, and identity operators.

# Keywords in Python — Detailed & Clear Explanation

Keywords in Python are reserved words that have a special meaning and cannot be used as variable names, function names, or identifiers.

📌 What are Keywords?

Keywords are predefined, reserved words in Python that define the syntax and structure of the language.

Example (❌ Invalid):

class = 10   # Error

🧠 Why Keywords Are Important?

They define program structure

They control flow of execution

They enable OOP, error handling, and imports

They are essential for writing valid Python code

📋 List of Python Keywords (Python 3.x)

Python currently has 35 keywords:

False  None  True
and  as  assert
break  class  continue
def  del  elif  else
except  finally  for
from  global  if
import  in  is
lambda  nonlocal  not
or  pass  raise
return  try  while
with  yield


📌 You can check keywords using:

import keyword
print(keyword.kwlist)

🔍 Keyword-wise Detailed Explanation
1️⃣ Value Keywords
🔹 True, False

Used for boolean values.

x = True
y = False

🔹 None

Represents no value / null.

x = None

2️⃣ Logical Keywords
🔹 and

Returns True if both conditions are true.

x > 5 and x < 10

🔹 or

Returns True if any one condition is true.

x > 5 or x > 20

🔹 not

Reverses the result.

not(x > 5)

3️⃣ Control Flow Keywords
🔹 if, elif, else

Used for decision making.

if x > 0:
    print("Positive")
elif x == 0:
    print("Zero")
else:
    print("Negative")

🔹 for

Used for looping.

for i in range(5):
    print(i)

🔹 while

Loop until condition is false.

while x < 5:
    x += 1

🔹 break

Stops loop execution.

break

🔹 continue

Skips current iteration.

continue

🔹 pass

Does nothing (placeholder).

if x > 0:
    pass

4️⃣ Function & Return Keywords
🔹 def

Used to define a function.

def add(a, b):
    return a + b

🔹 return

Returns a value from function.

return result

🔹 lambda

Creates an anonymous function.

square = lambda x: x * x

5️⃣ Object-Oriented Programming Keywords
🔹 class

Used to define a class.

class Student:
    pass

🔹 del

Deletes object or variable.

del x

🔹 global

Used to modify global variable inside function.

global x

🔹 nonlocal

Used to modify outer function variable.

nonlocal x

6️⃣ Exception Handling Keywords
🔹 try, except

Used to handle errors.

try:
    x = int("abc")
except ValueError:
    print("Error")

🔹 finally

Always executes.

finally:
    print("Done")

🔹 raise

Raises an exception manually.

raise ValueError("Invalid")

7️⃣ Import & Module Keywords
🔹 import

Imports module.

import math

🔹 from

Imports specific items.

from math import sqrt

🔹 as

Gives alias name.

import numpy as np

8️⃣ Membership & Identity Keywords
🔹 in

Checks presence.

'a' in 'apple'

🔹 is

Checks same memory reference.

a is b

9️⃣ Context & Generator Keywords
🔹 with

Used with file handling.

with open("file.txt") as f:
    data = f.read()

🔹 yield

Used in generators.

def count():
    yield 1

⚠️ Common Mistakes

❌ Using keywords as variable names
❌ Confusing is with ==
❌ Forgetting indentation with if, for, while

📌 Exam-Ready Definition

Keywords in Python are reserved words that have predefined meanings and are used to define the syntax and structure of the Python language. They cannot be used as identifiers.

# Data Types in Python — Detailed & Easy Explanation

A data type defines what kind of data a variable can store and what operations can be performed on it.

📌 What is a Data Type?

Data types specify the type of value stored in a variable.

Example:

x = 10        # int
y = 3.14      # float
name = "Ram"  # str


Python is dynamically typed, so the type is decided at runtime.

🧠 How to Check Data Type
x = 10
print(type(x))

🧱 Classification of Python Data Types

Python data types are broadly divided into:

1️⃣ Numeric
2️⃣ Sequence
3️⃣ Set
4️⃣ Mapping
5️⃣ Boolean
6️⃣ None

1️⃣ Numeric Data Types

Used to store numeric values.

🔹 (a) int (Integer)

Stores whole numbers.

x = 100
y = -25


✔ No size limit
✔ Supports large values

🔹 (b) float

Stores decimal numbers.

pi = 3.14

🔹 (c) complex

Stores complex numbers.

z = 2 + 3j


Access parts:

print(z.real)
print(z.imag)

2️⃣ Sequence Data Types

Used to store multiple values in sequence.

🔹 (a) str (String)

Stores text data.

name = "Python"


Features:

Immutable

Supports indexing & slicing

print(name[0])
print(name[1:4])

🔹 (b) list

Stores ordered, mutable collection.

numbers = [1, 2, 3, 4]
numbers.append(5)


✔ Allows duplicates
✔ Changeable

🔹 (c) tuple

Stores ordered, immutable collection.

t = (1, 2, 3)


✔ Faster than list
✔ Read-only

🔹 (d) range

Generates sequence of numbers.

r = range(1, 5)


Used in loops.

3️⃣ Set Data Types

Used to store unique values.

🔹 (a) set

Unordered and mutable.

s = {1, 2, 3}


✔ No duplicates
✔ Fast membership testing

🔹 (b) frozenset

Immutable version of set.

fs = frozenset([1, 2, 3])

4️⃣ Mapping Data Type
🔹 dict (Dictionary)

Stores data in key-value pairs.

student = {"name": "Amit", "age": 20}


✔ Keys are unique
✔ Mutable

Access value:

print(student["name"])

5️⃣ Boolean Data Type
🔹 bool

Stores True or False.

x = True
y = False


Used in conditions:

if x:
    print("True")

6️⃣ None Data Type
🔹 NoneType

Represents no value.

x = None


Used for initialization.

🔐 Mutable vs Immutable Data Types (Very Important)
🔹 Immutable

Cannot be changed after creation:

int

float

complex

str

tuple

frozenset

🔹 Mutable

Can be changed:

list

set

dict

🧪 Type Conversion (Type Casting)
🔹 Implicit Conversion
x = 10
y = 2.5
z = x + y   # float

🔹 Explicit Conversion
x = int("10")
y = float("3.5")

⚠️ Common Mistakes

❌ Confusing list with tuple
❌ Using mutable default arguments
❌ Assuming strings are mutable
❌ Forgetting type conversion

📌 Exam-Ready Definition

Data types in Python define the type of value a variable can store. Python supports numeric, sequence, set, mapping, boolean, and None data types.

# Conditional Statements in Python — Detailed Explanation

Conditional statements allow a program to make decisions and execute different blocks of code based on conditions.

📌 What are Conditional Statements?

Conditional statements are used to check conditions and execute code only if the condition is true.

Python uses:

if

if-else

if-elif-else

Nested if

🧠 How Conditions Work in Python

Conditions return True or False

Conditions use comparison & logical operators

Example:

x > 5
age >= 18 and age < 60

1️⃣ if Statement

Used when you want to execute code only if condition is true.

🔹 Syntax
if condition:
    statement

🔹 Example
age = 20

if age >= 18:
    print("Eligible to vote")


✔ If condition is false → nothing executes

2️⃣ if-else Statement

Used when you want two possible paths.

🔹 Syntax
if condition:
    statement1
else:
    statement2

🔹 Example
num = 5

if num % 2 == 0:
    print("Even")
else:
    print("Odd")

3️⃣ if-elif-else Statement

Used to check multiple conditions.

🔹 Syntax
if condition1:
    statement1
elif condition2:
    statement2
else:
    statement3

🔹 Example
marks = 75

if marks >= 90:
    print("Grade A")
elif marks >= 75:
    print("Grade B")
elif marks >= 60:
    print("Grade C")
else:
    print("Fail")


✔ Python checks conditions top to bottom
✔ First true condition executes

4️⃣ Nested if Statement

An if inside another if.

🔹 Example
age = 20
citizen = True

if age >= 18:
    if citizen:
        print("Eligible to vote")
    else:
        print("Not a citizen")
else:
    print("Underage")

🧮 Using Logical Operators in Conditions
🔹 and
age >= 18 and age <= 60

🔹 or
age < 18 or age > 60

🔹 not
not(age < 18)

🧪 Short-hand if (Ternary Operator)
🔹 Syntax
value_if_true if condition else value_if_false

🔹 Example
result = "Pass" if marks >= 40 else "Fail"

⚠️ Indentation (VERY IMPORTANT)

Python uses indentation instead of braces {}.

❌ Wrong:

if x > 0:
print("Positive")


✔ Correct:

if x > 0:
    print("Positive")

🔍 Truthy and Falsy Values
🔹 Falsy values
0, 0.0, "", None, [], {}, ()

🔹 Truthy values

Non-zero numbers

Non-empty strings, lists, tuples

Example:

if []:
    print("True")
else:
    print("False")

🧪 Example Program (Complete)
num = int(input("Enter number: "))

if num > 0:
    print("Positive")
elif num < 0:
    print("Negative")
else:
    print("Zero")

⚠️ Common Mistakes

❌ Using = instead of ==
❌ Wrong indentation
❌ Forgetting :
❌ Overusing nested if

📌 Exam-Ready Definition

Conditional statements in Python are used to make decisions by executing different blocks of code based on whether a condition is true or false.

# Loops in Python — Detailed & Easy Explanation

Loops are used to execute a block of code repeatedly until a condition is met or for a fixed number of times.

📌 What is a Loop?

A loop allows a program to repeat instructions automatically, reducing code repetition.

Python mainly provides:

for loop

while loop
(Loop control statements: break, continue, pass)

🧠 Why Loops Are Needed?

Avoid writing same code again and again

Process lists, strings, ranges

Used in DSA, ML, automation

1️⃣ for Loop

Used when the number of iterations is known.

🔹 Syntax
for variable in sequence:
    statements

🔹 Example 1: Basic for loop
for i in range(1, 6):
    print(i)

🔹 Example 2: Loop through list
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)

🔹 Example 3: Loop through string
for ch in "Python":
    print(ch)

🔢 range() Function (Very Important)
range(start, stop, step)


Examples:

range(5)          # 0 to 4
range(1, 6)       # 1 to 5
range(1, 10, 2)   # 1,3,5,7,9

2️⃣ while Loop

Used when the number of iterations is unknown and depends on a condition.

🔹 Syntax
while condition:
    statements

🔹 Example
i = 1
while i <= 5:
    print(i)
    i += 1


⚠️ Always update condition variable, otherwise infinite loop occurs.

3️⃣ Loop Control Statements
🔹 break

Stops the loop immediately.

for i in range(1, 10):
    if i == 5:
        break
    print(i)

🔹 continue

Skips current iteration.

for i in range(1, 6):
    if i == 3:
        continue
    print(i)

🔹 pass

Does nothing (placeholder).

for i in range(5):
    pass

4️⃣ Nested Loops

A loop inside another loop.

🔹 Example
for i in range(1, 4):
    for j in range(1, 4):
        print(i, j)

5️⃣ else with Loops (Unique Python Feature)
🔹 for-else

Executes else when loop completes normally.

for i in range(5):
    print(i)
else:
    print("Loop finished")


❌ else won’t execute if break is used.

6️⃣ Infinite Loop (Be Careful)
while True:
    print("Hello")


Used intentionally in:

Servers

Games

Input validation

7️⃣ Real-World Examples
🔹 Sum of numbers
sum = 0
for i in range(1, 6):
    sum += i
print(sum)

🔹 Factorial using while
n = 5
fact = 1
while n > 0:
    fact *= n
    n -= 1
print(fact)

⚠️ Common Mistakes

❌ Infinite loop
❌ Wrong indentation
❌ Forgetting to update loop variable
❌ Using range() incorrectly

📌 Exam-Ready Definition

Loops in Python are used to execute a block of code repeatedly based on a condition or sequence.

# Functions in Python — Deep & Complete Explanation

A function in Python is a block of reusable code that performs a specific task.
Functions help make programs modular, readable, reusable, and easy to debug.

📌 What is a Function?

A function is a named block of code that executes only when it is called and may return a value.

🔹 Example
def greet():
    print("Hello Python")

greet()

🧠 Why Functions Are Important?

Avoid code repetition

Break large programs into small parts

Improve readability

Easy debugging & testing

Essential for DSA, ML, Web Dev

🧱 Types of Functions in Python

1️⃣ Built-in functions
2️⃣ User-defined functions
3️⃣ Anonymous (Lambda) functions

1️⃣ Built-in Functions

Already provided by Python.

Examples:

print()
len()
type()
sum()
range()

2️⃣ User-Defined Functions

Created using def keyword.

🔹 Syntax of a Function
def function_name(parameters):
    statements
    return value

🔹 Function Without Parameters
def show():
    print("Welcome")

show()

🔹 Function With Parameters
def add(a, b):
    return a + b

print(add(5, 3))

🔁 Parameters vs Arguments
Parameters	Arguments
Variables in function definition	Actual values passed
a, b	5, 3
🧮 Types of Arguments (Very Important)
1️⃣ Positional Arguments

Order matters.

def sub(a, b):
    return a - b

sub(10, 5)

2️⃣ Keyword Arguments

Order doesn’t matter.

sub(b=5, a=10)

3️⃣ Default Arguments

Default value is used if no argument passed.

def greet(name="User"):
    print("Hello", name)

greet()
greet("Amit")

4️⃣ Variable-Length Arguments
🔹 *args (Non-keyword arguments)
def add(*args):
    return sum(args)

print(add(1, 2, 3))

🔹 **kwargs (Keyword arguments)
def info(**kwargs):
    print(kwargs)

info(name="Ram", age=20)

🔄 Return Statement

Used to send value back to caller.

def square(x):
    return x * x


Multiple returns:

def calc(a, b):
    return a+b, a-b

🔍 Scope of Variables in Functions (LEGB Rule)

1️⃣ Local
2️⃣ Enclosing
3️⃣ Global
4️⃣ Built-in

🔹 Local Variable
def f():
    x = 10

🔹 Global Variable
x = 20

def f():
    global x
    x = 30

🧩 Lambda (Anonymous) Functions

Functions without name, written in one line.

🔹 Syntax
lambda arguments: expression

🔹 Example
square = lambda x: x*x
print(square(5))


✔ Used in map(), filter(), reduce()

🔁 Recursive Functions

Function calling itself.

🔹 Example: Factorial
def fact(n):
    if n == 0:
        return 1
    return n * fact(n-1)

📄 Docstrings (Function Documentation)
def add(a, b):
    """Returns sum of two numbers"""
    return a + b


Access:

print(add.__doc__)

🧪 Real-World Example
def calculate_bill(price, tax=5):
    return price + (price * tax / 100)

print(calculate_bill(100))

⚠️ Common Mistakes

❌ Forgetting return
❌ Confusing parameters & arguments
❌ Using mutable default arguments
❌ Infinite recursion

📌 Exam-Ready Definition

A function in Python is a reusable block of code defined using the def keyword that performs a specific task and may return a value.

# ## 🟡 `pass` Statement in Python Functions — **Detailed Explanation**

The **`pass` statement** in Python is a **null (do-nothing) statement**.
It is used when a statement is **syntactically required**, but **no action is needed** at that moment.

---

## 📌 What is `pass`?

> `pass` is a placeholder statement that allows you to write empty blocks of code without causing syntax errors.

Python does **not allow empty blocks**, so `pass` is used to avoid errors.

---

## 🔹 Why `pass` is Needed in Functions?

When defining a function, Python expects **at least one statement** inside the function body.

❌ Invalid:

```python
def my_func():
```

✔ Valid using `pass`:

```python
def my_func():
    pass
```

---

## 🧠 Key Characteristics of `pass`

* Does **nothing**
* Produces **no output**
* Does **not stop execution**
* Used as a **temporary placeholder**
* Often used during **development or design**

---

## 🧩 `pass` Statement in Functions

### 🔹 Example 1: Empty Function

```python
def future_function():
    pass
```

✔ Program runs without error
✔ Function does nothing when called

```python
future_function()
```

---

### 🔹 Example 2: Function Skeleton (Real Use Case)

```python
def login():
    pass

def register():
    pass
```

👉 Used when planning program structure before implementation.

---

## 🔁 `pass` vs `return` (Very Important Difference)

| `pass`              | `return`         |
| ------------------- | ---------------- |
| Does nothing        | Sends value back |
| Execution continues | Exits function   |
| Used as placeholder | Used for result  |

Example:

```python
def f1():
    pass

def f2():
    return
```

---

## 🔄 `pass` vs `break` vs `continue`

| Keyword    | Effect          |
| ---------- | --------------- |
| `pass`     | Does nothing    |
| `break`    | Stops loop      |
| `continue` | Skips iteration |

Example:

```python
for i in range(3):
    if i == 1:
        pass
    print(i)
```

Output:

```
0
1
2
```

---

## 🧪 `pass` in Conditional Statements inside Functions

```python
def check(x):
    if x > 0:
        pass
    else:
        print("Negative or zero")
```

✔ Useful when logic is incomplete

---

## 🧱 `pass` in Class & Function Design

```python
class Student:
    pass
```

✔ Used when defining class structure

---

## ⚠️ Common Mistakes

❌ Thinking `pass` stops execution
❌ Expecting output from `pass`
❌ Confusing `pass` with `return`

---

## 📌 Exam-Ready Definition

> The `pass` statement in Python is a null statement used as a placeholder where a statement is required syntactically but no action is to be performed.

---

# ## 🌍 Global and Local Variables in Python — **Detailed Explanation**

In Python, **scope** defines **where a variable can be accessed**.
The two most important scopes are **Local** and **Global**.

---

## 📌 What is Variable Scope?

> Variable scope determines the part of the program where a variable is accessible.

Python follows the **LEGB rule**:

* **L**ocal
* **E**nclosing
* **G**lobal
* **B**uilt-in

(We’ll focus mainly on **Local** and **Global** here.)

---

## 1️⃣ Local Variables

### 🔹 Definition

A **local variable** is a variable **declared inside a function**.
It is **accessible only within that function**.

---

### 🔹 Example

```python
def show():
    x = 10      # local variable
    print(x)

show()
```

✔ `x` exists only inside `show()`
❌ Cannot be accessed outside the function

```python
print(x)   # Error
```

---

### 🔹 Key Points of Local Variables

* Created when function is called
* Destroyed after function execution
* Safe from outside modification
* Helps avoid name conflicts

---

## 2️⃣ Global Variables

### 🔹 Definition

A **global variable** is a variable **declared outside all functions**.
It is **accessible throughout the program**.

---

### 🔹 Example

```python
x = 20   # global variable

def show():
    print(x)

show()
print(x)
```

✔ Accessible inside and outside functions

---

### 🔹 Using Global Variable Inside Function (Read Only)

You can **read** a global variable inside a function **without any keyword**.

---

## 3️⃣ Modifying Global Variable Inside Function (`global` keyword)

By default, **you cannot modify** a global variable inside a function.

❌ Error Example:

```python
x = 10

def update():
    x = x + 5   # Error

update()
```

---

### ✔ Correct Way Using `global`

```python
x = 10

def update():
    global x
    x = x + 5

update()
print(x)
```

---

### 🔹 What `global` Does?

* Tells Python to use the **global variable**
* Avoids creation of local variable with same name

---

## 4️⃣ Local vs Global Variable (Same Name)

```python
x = 50

def test():
    x = 10
    print(x)

test()
print(x)
```

Output:

```
10
50
```

✔ Local variable hides global variable inside function

---

## 5️⃣ Enclosing Variable (Short Introduction)

Used in **nested functions**.

```python
def outer():
    x = 20
    def inner():
        print(x)
    inner()

outer()
```

---

### 🔹 `nonlocal` Keyword

Used to modify enclosing variable.

```python
def outer():
    x = 10
    def inner():
        nonlocal x
        x = 20
    inner()
    print(x)

outer()
```

---

## 6️⃣ Built-in Scope (Just for Awareness)

Built-in names like:

```python
print()
len()
sum()
```

Avoid overwriting:

```python
print = 5   # Bad practice
```

---

## 🔍 LEGB Rule Example

```python
x = 100

def outer():
    x = 50
    def inner():
        x = 10
        print(x)
    inner()

outer()
```

Python searches:

1. Local (`inner`)
2. Enclosing (`outer`)
3. Global
4. Built-in

---

## ⚠️ Common Mistakes

❌ Forgetting `global` keyword
❌ Confusing local with global
❌ Overusing global variables
❌ Shadowing built-in names

---

## 📌 Exam-Ready Definition

> A local variable is declared inside a function and accessible only within that function, whereas a global variable is declared outside all functions and accessible throughout the program.

---

## 📝 Short Exam Answer

> Global variables are declared outside functions and can be accessed anywhere in the program. Local variables are declared inside functions and are accessible only within that function.

---

## 🎯 Why This Topic Is Important for You

* Frequently asked in **BCA exams**
* Essential for **functions & DSA**
* Important for **ML model code**
* Asked in **interviews**

---

If you want next:
✅ **LEGB rule with diagrams**
✅ **Global vs nonlocal difference**
✅ **MCQs & practice programs**
✅ **README.md formatted notes**

Just tell me 👍

# ## 🔄 Recursion in Python — **Detailed Explanation**

**Recursion** is a programming technique where a **function calls itself** to solve a problem. It is widely used in **mathematics, algorithms, and computer science**.

---

## 📌 What is Recursion?

> Recursion is a method of solving a problem where the solution depends on **smaller instances of the same problem**, and a function calls itself to achieve this.

---

### 🔹 Structure of a Recursive Function

1. **Base Case** – The condition to stop recursion
2. **Recursive Case** – The function calls itself with a smaller problem

```python
def recursive_function():
    if base_condition:
        return
    else:
        recursive_function()   # recursive call
```

---

## 1️⃣ Example: Factorial Using Recursion

Factorial of `n` (n!) = n × (n-1) × (n-2) ... × 1

```python
def factorial(n):
    if n == 0 or n == 1:   # Base case
        return 1
    else:
        return n * factorial(n-1)  # Recursive case

print(factorial(5))  # Output: 120
```

**Explanation:**

* factorial(5) calls factorial(4)
* factorial(4) calls factorial(3) …
* Base case factorial(0) returns 1

---

## 2️⃣ Example: Fibonacci Sequence Using Recursion

Fibonacci: 0, 1, 1, 2, 3, 5, 8…

```python
def fibonacci(n):
    if n == 0:
        return 0
    elif n == 1:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)

for i in range(6):
    print(fibonacci(i), end=" ")
```

Output:

```
0 1 1 2 3 5
```

---

## 3️⃣ How Recursion Works (Step-by-Step)

For factorial(3):

1. factorial(3) = 3 * factorial(2)
2. factorial(2) = 2 * factorial(1)
3. factorial(1) = 1 (base case)
4. Return values propagate: 2 * 1 → 3 * 2 → 6

This is called **recursion tree expansion and contraction**.

---

## 4️⃣ Types of Recursion

1. **Direct Recursion** – Function calls itself directly
2. **Indirect Recursion** – Function A calls B, and B calls A
3. **Tail Recursion** – Recursive call is the last statement
4. **Non-Tail Recursion** – Recursive call is not the last statement

---

## 5️⃣ Advantages of Recursion

* Simplifies **complex problems** like tree traversal, factorial, Fibonacci
* Reduces **code length**
* Useful in **divide-and-conquer algorithms** (Merge Sort, Quick Sort)

---

## 6️⃣ Disadvantages of Recursion

* **Consumes more memory** (stack space)
* Can lead to **stack overflow** if base case is missing
* Slower than iterative solutions sometimes

---

## 7️⃣ Example: Sum of N Numbers Using Recursion

```python
def sum_n(n):
    if n == 0:
        return 0
    else:
        return n + sum_n(n-1)

print(sum_n(5))  # Output: 15
```

---

## 8️⃣ Important Notes

* Always define a **base case**, otherwise **infinite recursion** occurs
* Recursive functions can **call themselves multiple times**
* Python has a **maximum recursion depth** (`sys.getrecursionlimit()` ≈ 1000)

---

## ⚠️ Common Mistakes

❌ Missing base case → infinite recursion
❌ Changing the wrong variable
❌ Using recursion where iteration is simpler
❌ Forgetting to return values

---

## 📌 Exam-Ready Definition

> Recursion in Python is a technique where a function calls itself to solve smaller instances of a problem until a base case is reached.

---

## 📝 Short Example for Exams

```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)
```

---

## 🎯 Why Recursion Is Important for You

* Core for **DSA** (trees, graphs)
* Used in **mathematical algorithms**
* Helps in **ML algorithm implementation**
* Frequently asked in **BCA exams & interviews**

---

If you want next:
✅ **Recursion flowchart + diagram**
✅ **Tail vs Non-Tail Recursion**
✅ **Recursion practice problems**
✅ **README.md formatted notes with examples**

Do you want me to make **all recursion examples in one visual diagram** for easy understanding?

# ## 🔄 Recursion in Python — **Detailed Explanation**

**Recursion** is a programming technique where a **function calls itself** to solve a problem. It is widely used in **mathematics, algorithms, and computer science**.

---

## 📌 What is Recursion?

> Recursion is a method of solving a problem where the solution depends on **smaller instances of the same problem**, and a function calls itself to achieve this.

---

### 🔹 Structure of a Recursive Function

1. **Base Case** – The condition to stop recursion
2. **Recursive Case** – The function calls itself with a smaller problem

```python
def recursive_function():
    if base_condition:
        return
    else:
        recursive_function()   # recursive call
```

---

## 1️⃣ Example: Factorial Using Recursion

Factorial of `n` (n!) = n × (n-1) × (n-2) ... × 1

```python
def factorial(n):
    if n == 0 or n == 1:   # Base case
        return 1
    else:
        return n * factorial(n-1)  # Recursive case

print(factorial(5))  # Output: 120
```

**Explanation:**

* factorial(5) calls factorial(4)
* factorial(4) calls factorial(3) …
* Base case factorial(0) returns 1

---

## 2️⃣ Example: Fibonacci Sequence Using Recursion

Fibonacci: 0, 1, 1, 2, 3, 5, 8…

```python
def fibonacci(n):
    if n == 0:
        return 0
    elif n == 1:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)

for i in range(6):
    print(fibonacci(i), end=" ")
```

Output:

```
0 1 1 2 3 5
```

---

## 3️⃣ How Recursion Works (Step-by-Step)

For factorial(3):

1. factorial(3) = 3 * factorial(2)
2. factorial(2) = 2 * factorial(1)
3. factorial(1) = 1 (base case)
4. Return values propagate: 2 * 1 → 3 * 2 → 6

This is called **recursion tree expansion and contraction**.

---

## 4️⃣ Types of Recursion

1. **Direct Recursion** – Function calls itself directly
2. **Indirect Recursion** – Function A calls B, and B calls A
3. **Tail Recursion** – Recursive call is the last statement
4. **Non-Tail Recursion** – Recursive call is not the last statement

---

## 5️⃣ Advantages of Recursion

* Simplifies **complex problems** like tree traversal, factorial, Fibonacci
* Reduces **code length**
* Useful in **divide-and-conquer algorithms** (Merge Sort, Quick Sort)

---

## 6️⃣ Disadvantages of Recursion

* **Consumes more memory** (stack space)
* Can lead to **stack overflow** if base case is missing
* Slower than iterative solutions sometimes

---

## 7️⃣ Example: Sum of N Numbers Using Recursion

```python
def sum_n(n):
    if n == 0:
        return 0
    else:
        return n + sum_n(n-1)

print(sum_n(5))  # Output: 15
```

---

## 8️⃣ Important Notes

* Always define a **base case**, otherwise **infinite recursion** occurs
* Recursive functions can **call themselves multiple times**
* Python has a **maximum recursion depth** (`sys.getrecursionlimit()` ≈ 1000)

---

## ⚠️ Common Mistakes

❌ Missing base case → infinite recursion
❌ Changing the wrong variable
❌ Using recursion where iteration is simpler
❌ Forgetting to return values

---

## 📌 Exam-Ready Definition

> Recursion in Python is a technique where a function calls itself to solve smaller instances of a problem until a base case is reached.

---

## 📝 Short Example for Exams

```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)
```

---

## 🎯 Why Recursion Is Important for You

* Core for **DSA** (trees, graphs)
* Used in **mathematical algorithms**
* Helps in **ML algorithm implementation**
* Frequently asked in **BCA exams & interviews**

---

If you want next:
✅ **Recursion flowchart + diagram**
✅ **Tail vs Non-Tail Recursion**
✅ **Recursion practice problems**
✅ **README.md formatted notes with examples**

Do you want me to make **all recursion examples in one visual diagram** for easy understanding?

# ## 📦 `*args` and `**kwargs` in Python Functions — **Detailed Explanation**

In Python, `*args` and `**kwargs` are used to **pass variable-length arguments** to a function.
They make functions **flexible** and allow handling of **unknown number of inputs**.

---

## 1️⃣ `*args` — Variable-Length Positional Arguments

### 🔹 What is `*args`?

> `*args` allows a function to accept **any number of positional arguments** as a **tuple**.

---

### 🔹 Syntax

```python
def function_name(*args):
    # args is a tuple
    for item in args:
        print(item)
```

---

### 🔹 Example

```python
def add_numbers(*args):
    return sum(args)

print(add_numbers(1, 2, 3))      # Output: 6
print(add_numbers(5, 10, 15, 20)) # Output: 50
```

---

### 🔹 Key Points

* Arguments passed are **positional**
* Stored as a **tuple** inside function
* Can combine with **normal arguments**:

```python
def greet(greeting, *names):
    print(greeting, end=" ")
    for name in names:
        print(name, end=" ")
```

---

## 2️⃣ `**kwargs` — Variable-Length Keyword Arguments

### 🔹 What is `**kwargs`?

> `**kwargs` allows a function to accept **any number of keyword arguments** as a **dictionary**.

---

### 🔹 Syntax

```python
def function_name(**kwargs):
    for key, value in kwargs.items():
        print(key, "=", value)
```

---

### 🔹 Example

```python
def student_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

student_info(name="Amit", age=20, course="BCA")
```

Output:

```
name: Amit
age: 20
course: BCA
```

---

### 🔹 Key Points

* Arguments are passed as **key=value**
* Stored as a **dictionary**
* Can combine with **normal arguments** and `*args`:

```python
def display(a, b, *args, **kwargs):
    print(a, b)
    print(args)
    print(kwargs)
```

---

## 3️⃣ Combining Normal, `*args`, and `**kwargs`

Order of parameters in function definition:

```python
def func(normal1, normal2, *args, **kwargs):
    pass
```

### 🔹 Example

```python
def demo(a, b, *args, **kwargs):
    print("a =", a)
    print("b =", b)
    print("args =", args)
    print("kwargs =", kwargs)

demo(1, 2, 3, 4, 5, x=10, y=20)
```

Output:

```
a = 1
b = 2
args = (3, 4, 5)
kwargs = {'x': 10, 'y': 20}
```

---

## 4️⃣ Unpacking with `*` and `**`

### 🔹 Example 1: Unpacking list/tuple with `*`

```python
numbers = [1, 2, 3]
print(*numbers)   # Output: 1 2 3
```

### 🔹 Example 2: Unpacking dictionary with `**`

```python
data = {'name': 'Amit', 'age': 20}
def info(name, age):
    print(name, age)

info(**data)       # Output: Amit 20
```

---

## 5️⃣ Use Cases

* **`*args`** → when number of **positional arguments** is unknown
* **`**kwargs`** → when number of **keyword arguments** is unknown
* Helpful in **API functions, wrappers, decorators, and flexible functions**

---

## ⚠️ Common Mistakes

* Wrong order of arguments

```python
def f(*args, a):  # ❌
    pass
```

* Forgetting `*` or `**` when unpacking
* Using `*args` and `**kwargs` in the wrong order

---

## 📌 Exam-Ready Definition

> `*args` in Python allows passing a variable number of **positional arguments** to a function as a **tuple**, while `**kwargs` allows passing a variable number of **keyword arguments** as a **dictionary**.

---

## 📝 Short Example for Exams

```python
def func(*args, **kwargs):
    print(args)
    print(kwargs)

func(1,2,3, x=10, y=20)
```

Output:

```
(1, 2, 3)
{'x': 10, 'y': 20}
```

---

## 🎯 Why This Topic Is Important

* Used in **Python libraries and frameworks**
* Essential for **flexible function design**
* Frequently asked in **BCA exams & interviews**
* Core for **decorators and advanced Python concepts**

---

If you want next:
✅ **Decorators in Python explained**
✅ **Practical examples combining `*args` and `**kwargs`**
✅ **README.md formatted notes with examples**

Do you want me to make **a full visual diagram showing `*args` and `**kwargs` usage**?

# ## 🟢 `self` as Default Argument in Python — **Detailed Explanation**

In Python, **`self`** is a reference to the **current instance of a class**. It is used to **access instance variables and methods** from within a class.

---

## 📌 What is `self`?

> `self` represents the **object itself**. When you create an object of a class, Python automatically passes the object to methods as the **first argument**, which by convention is named `self`.

* It is **not a keyword**, but a **strong convention**.
* Always comes as the **first parameter** in instance methods.

---

## 🔹 Why `self` is Needed?

* To access **instance variables** inside methods
* To differentiate between **local and instance variables**
* To call **other methods of the same class**
* Required for **object-oriented programming** in Python

---

## 1️⃣ Example: Using `self` in a Class

```python
class Student:
    def __init__(self, name, age):
        self.name = name   # instance variable
        self.age = age

    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)

# Creating object
s1 = Student("Amit", 20)
s1.display()
```

**Explanation:**

* `self.name` and `self.age` are **instance variables**.
* `s1` is passed as `self` automatically to methods.
* `display()` accesses instance variables via `self`.

---

## 2️⃣ `self` is Automatically Passed

```python
class Test:
    def hello(self):
        print("Hello")

t = Test()
t.hello()
```

Equivalent to:

```python
Test.hello(t)  # `t` is passed as `self`
```

So, `self` allows **object context** inside methods.

---

## 3️⃣ Using `self` to Access Other Methods

```python
class Student:
    def greet(self):
        print("Hello")

    def message(self):
        print("Welcome")
        self.greet()  # calling another method using self

s = Student()
s.message()
```

Output:

```
Welcome
Hello
```

---

## 4️⃣ Difference Between `self` and Default Arguments

* **`self` is not optional** in instance methods. Python automatically passes it when calling via object.
* **Default arguments** are optional parameters with default values.

```python
class Test:
    def add(self, a=5, b=10):  # a & b are default arguments
        print(a + b)

t = Test()
t.add()          # Output: 15
t.add(20, 30)    # Output: 50
```

---

## 5️⃣ Important Points About `self`

1. First parameter in instance methods
2. Represents **current object**
3. Can access **instance variables & methods**
4. Can be named differently, but **`self` is standard**

```python
class Demo:
    def show(obj):  # valid but not recommended
        print(obj)
```

---

## 6️⃣ Common Mistakes

❌ Forgetting `self` in method definition

```python
class Test:
    def greet():   # Error
        print("Hello")
```

❌ Using `self` outside class context
❌ Not understanding that `self` allows method to access instance data

---

## 📌 Exam-Ready Definition

> `self` in Python is a reference to the current object of a class. It is used to access **instance variables and methods** inside class methods and is automatically passed when the method is called via an object.

---

## 📝 Short Example for Exams

```python
class Student:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print("Hello", self.name)

s = Student("Amit")
s.greet()
```

Output:

```
Hello Amit
```

---

## 🎯 Why This Topic Is Important

* Core concept in **OOP in Python**
* Required for **BCA exams**
* Essential for **method and class design**
* Frequently asked in **interviews**

---

If you want next:
✅ **Class vs Object vs self diagram**
✅ **Instance vs Class variables with self**
✅ **README.md formatted notes**

Do you want me to make **a full visual diagram showing `self` usage**?

# ## 🌟 First-Class Functions in Python — **Detailed Explanation**

In Python, **functions are first-class citizens**, which means they can be **treated like any other object** (like integers, strings, lists, etc.).

---

## 📌 What is a First-Class Function?

> A **first-class function** is a function that can be:

1. **Assigned to a variable**
2. **Passed as an argument** to another function
3. **Returned from another function**
4. **Stored in data structures** (list, dict, etc.)

This is a **core concept of functional programming** in Python.

---

## 1️⃣ Assigning Function to a Variable

```python
def greet(name):
    return f"Hello, {name}!"

# Assign function to a variable
say_hello = greet

print(say_hello("Amit"))  # Output: Hello, Amit!
```

**Explanation:**

* `greet` is assigned to `say_hello`
* `say_hello` can be called like the original function

---

## 2️⃣ Passing Function as Argument

```python
def greet(name):
    return f"Hello, {name}!"

def welcome(func, name):
    print(func(name))

welcome(greet, "Amit")  # Output: Hello, Amit!
```

**Explanation:**

* `greet` is passed as an argument to `welcome`
* This allows **higher-order functions**

---

## 3️⃣ Returning Function from Another Function

```python
def outer():
    def inner():
        return "I am inner function"
    return inner

f = outer()
print(f())  # Output: I am inner function
```

**Explanation:**

* `outer()` returns `inner` function
* `f` now holds `inner`, which can be called

---

## 4️⃣ Storing Functions in Data Structures

```python
def add(a, b):
    return a + b

def sub(a, b):
    return a - b

func_list = [add, sub]

print(func_list[0](10, 5))  # Output: 15
print(func_list[1](10, 5))  # Output: 5
```

---

## 5️⃣ Practical Example: Higher-Order Function

```python
def square(x):
    return x*x

def cube(x):
    return x**3

def apply_func(func, value):
    return func(value)

print(apply_func(square, 5))  # Output: 25
print(apply_func(cube, 3))    # Output: 27
```

**Explanation:**

* `apply_func` accepts **any function** and a value
* Demonstrates **flexible code design**

---

## 6️⃣ First-Class Functions vs Regular Functions

| Feature    | First-Class Function             | Regular Function        |
| ---------- | -------------------------------- | ----------------------- |
| Assignment | Can assign to variable           | Not necessary           |
| Passing    | Can pass as argument             | Usually called directly |
| Returning  | Can return from another function | Usually returns a value |
| Storage    | Can store in data structures     | Not necessary           |

---

## 7️⃣ Advantages of First-Class Functions

* **Code reusability** – Functions can be passed around
* **Flexible APIs** – Functions as parameters
* **Functional programming** – Map, filter, reduce
* **Dynamic behavior** – Can select functions at runtime

---

## 8️⃣ Key Concepts Related to First-Class Functions

* **Higher-Order Function** – Function that **accepts or returns another function**
* **Anonymous Functions (`lambda`)** – Often used with first-class functions
* **Closures** – Inner function retains access to outer function’s variables

---

## 9️⃣ Example with Lambda and First-Class Function

```python
def apply_func(func, value):
    return func(value)

print(apply_func(lambda x: x*2, 10))  # Output: 20
```

---

## ⚠️ Common Mistakes

* Forgetting to pass **function reference** instead of calling it (`func` vs `func()`)
* Returning function but **forgetting parentheses** when calling
* Confusing **first-class function** with **method chaining**

---

## 📌 Exam-Ready Definition

> A first-class function in Python is a function that can be **assigned to variables, passed as arguments, returned from other functions, and stored in data structures**, just like any other object.

---

## 📝 Short Example for Exams

```python
def greet(name):
    return f"Hello, {name}"

say_hello = greet          # Assign
print(say_hello("Amit"))   # Call
```

---

## 🎯 Why This Topic Is Important

* Core concept in **functional programming**
* Required for **decorators, closures, and callbacks**
* Frequently asked in **BCA exams & Python interviews**
* Essential for **writing flexible Python code**

---

If you want next:
✅ **Closures in Python explained**
✅ **Decorators using first-class functions**
✅ **README.md formatted notes with diagrams**

Do you want me to make **a full diagram showing first-class functions, higher-order functions, and closures**?

# ## 🌟 Lambda Function in Python — **Detailed Explanation**

A **lambda function** in Python is a **small anonymous function** that is defined without a name.
It can take any number of arguments but has **only one expression**. The result of the expression is **automatically returned**.

---

## 📌 What is a Lambda Function?

> A **lambda function** is a quick, inline function defined using the `lambda` keyword, usually used for **short, simple tasks**.

---

### 🔹 Syntax

```python
lambda arguments: expression
```

* `lambda` – keyword
* `arguments` – parameters passed to the function
* `expression` – single expression evaluated and returned

---

## 1️⃣ Example: Simple Lambda Function

```python
square = lambda x: x * x
print(square(5))  # Output: 25
```

**Explanation:**

* `x` is the argument
* `x * x` is the expression
* `square` is the variable storing the lambda function

---

## 2️⃣ Lambda with Multiple Arguments

```python
add = lambda a, b: a + b
print(add(10, 20))  # Output: 30
```

---

## 3️⃣ Lambda in Place of Normal Functions

**Normal Function:**

```python
def square(x):
    return x * x
```

**Lambda Function:**

```python
square = lambda x: x * x
```

✅ Both behave the same, but **lambda is more concise**.

---

## 4️⃣ Using Lambda with `map()`

`map()` applies a function to each item of an iterable.

```python
nums = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x**2, nums))
print(squared)  # Output: [1, 4, 9, 16, 25]
```

---

## 5️⃣ Using Lambda with `filter()`

`filter()` filters items from an iterable based on a condition.

```python
nums = [1, 2, 3, 4, 5, 6]
even_nums = list(filter(lambda x: x % 2 == 0, nums))
print(even_nums)  # Output: [2, 4, 6]
```

---

## 6️⃣ Using Lambda with `reduce()`

`reduce()` (from `functools`) reduces a list to a single value.

```python
from functools import reduce

nums = [1, 2, 3, 4]
sum_nums = reduce(lambda x, y: x + y, nums)
print(sum_nums)  # Output: 10
```

---

## 7️⃣ Lambda in `sorted()` or `sort()`

Sorting list of tuples by the second element:

```python
data = [(1, 'b'), (2, 'a'), (3, 'c')]
sorted_data = sorted(data, key=lambda x: x[1])
print(sorted_data)  # Output: [(2, 'a'), (1, 'b'), (3, 'c')]
```

---

## 8️⃣ Advantages of Lambda Functions

* **Concise** and readable for simple functions
* Useful in **functional programming** (`map`, `filter`, `reduce`)
* Can be passed as **arguments to other functions**
* No need to **define a named function** for short tasks

---

## 9️⃣ Limitations of Lambda Functions

* Can contain **only one expression**
* Cannot include statements (loops, `print`, etc.)
* Less readable for **complex logic**
* Cannot have **annotations or docstrings**

---

## 10️⃣ Lambda vs Regular Function

| Feature    | Lambda                 | Regular Function    |
| ---------- | ---------------------- | ------------------- |
| Syntax     | `lambda x: x*x`        | `def square(x):`    |
| Name       | Anonymous (optional)   | Named               |
| Statements | Single expression only | Multiple statements |
| Usage      | Short/simple tasks     | Complex logic       |

---

## 11️⃣ Practical Example: First-Class Functions

```python
def apply_func(func, value):
    return func(value)

result = apply_func(lambda x: x*3, 5)
print(result)  # Output: 15
```

**Explanation:**

* Lambda is passed as an argument to a higher-order function
* Avoids creating a separate named function

---

## ⚠️ Common Mistakes

* Using **multiple statements** → ❌ not allowed
* Forgetting to assign lambda if you want to reuse
* Overusing lambda for complex functions → reduces readability

---

## 📌 Exam-Ready Definition

> A lambda function in Python is an **anonymous function** defined using the `lambda` keyword, capable of taking any number of arguments but containing only a **single expression**, which is returned automatically.

---

## 📝 Short Example for Exams

```python
square = lambda x: x*x
print(square(5))  # Output: 25
```

---

## 🎯 Why This Topic Is Important

* Essential for **functional programming** in Python
* Used in **map, filter, reduce, sorted**
* Core for **first-class functions and decorators**
* Frequently asked in **BCA exams & interviews**

---

If you want next:
✅ **Closures in Python explained**
✅ **Decorators using lambda functions**
✅ **README.md formatted notes with examples**

Do you want me to **make a visual diagram showing lambda, map, filter, reduce, and first-class function together**?

# ## 🔹 Map, Filter, and Reduce Functions in Python — **Detailed Explanation**

Python provides **built-in functions** `map()` and `filter()`, and a function `reduce()` in the `functools` module, which are commonly used in **functional programming**.
They allow you to **process iterables efficiently** using functions, often **lambda functions**.

---

## 1️⃣ `map()` Function

### 🔹 What is `map()`?

> `map()` applies a given function to **all items in an iterable** (like list, tuple) and returns a **map object** (can be converted to list, tuple, etc.).

---

### 🔹 Syntax

```python
map(function, iterable)
```

* **function** – function to apply (can be `lambda`)
* **iterable** – list, tuple, etc.

---

### 🔹 Example 1: Square of numbers

```python
nums = [1, 2, 3, 4, 5]
squared = map(lambda x: x**2, nums)
print(list(squared))  # Output: [1, 4, 9, 16, 25]
```

---

### 🔹 Example 2: Uppercase strings

```python
words = ['apple', 'banana', 'mango']
upper_words = map(str.upper, words)
print(list(upper_words))  # Output: ['APPLE', 'BANANA', 'MANGO']
```

---

### 🔹 Key Points about `map()`

* Returns a **map object**
* Can use **named function or lambda**
* Useful for **applying the same operation** to all elements

---

## 2️⃣ `filter()` Function

### 🔹 What is `filter()`?

> `filter()` filters elements of an iterable **based on a function that returns True or False**.

---

### 🔹 Syntax

```python
filter(function, iterable)
```

* **function** – returns `True` or `False`
* **iterable** – list, tuple, etc.

---

### 🔹 Example 1: Filter even numbers

```python
nums = [1, 2, 3, 4, 5, 6]
even_nums = filter(lambda x: x % 2 == 0, nums)
print(list(even_nums))  # Output: [2, 4, 6]
```

---

### 🔹 Example 2: Filter strings starting with 'a'

```python
words = ['apple', 'banana', 'avocado', 'mango']
a_words = filter(lambda x: x[0] == 'a', words)
print(list(a_words))  # Output: ['apple', 'avocado']
```

---

### 🔹 Key Points about `filter()`

* Returns a **filter object**
* Keeps elements where function returns `True`
* Often used with **lambda functions**

---

## 3️⃣ `reduce()` Function

### 🔹 What is `reduce()`?

> `reduce()` **reduces a list to a single value** by applying a function cumulatively to its items.

* Example: sum, product, factorial
* Available in `functools` module

---

### 🔹 Syntax

```python
from functools import reduce
reduce(function, iterable)
```

---

### 🔹 Example 1: Sum of numbers

```python
from functools import reduce

nums = [1, 2, 3, 4, 5]
total = reduce(lambda x, y: x + y, nums)
print(total)  # Output: 15
```

**Explanation:**

* Step 1: 1 + 2 = 3
* Step 2: 3 + 3 = 6
* Step 3: 6 + 4 = 10
* Step 4: 10 + 5 = 15

---

### 🔹 Example 2: Product of numbers

```python
nums = [1, 2, 3, 4]
product = reduce(lambda x, y: x * y, nums)
print(product)  # Output: 24
```

---

### 🔹 Key Points about `reduce()`

* Returns a **single value**
* Takes **two arguments** in the lambda
* Performs **cumulative operation**

---

## 4️⃣ Comparison Table

| Function   | Returns       | Usage                           | Example                                  |
| ---------- | ------------- | ------------------------------- | ---------------------------------------- |
| `map()`    | Map object    | Apply function to all items     | `map(lambda x:x*2, [1,2,3])` → [2,4,6]   |
| `filter()` | Filter object | Filter items based on condition | `filter(lambda x:x%2==0, [1,2,3])` → [2] |
| `reduce()` | Single value  | Reduce iterable to one value    | `reduce(lambda x,y:x+y, [1,2,3])` → 6    |

---

## 5️⃣ Practical Example: Combined Use

```python
from functools import reduce

nums = [1, 2, 3, 4, 5, 6]

# Step 1: Filter even numbers
evens = filter(lambda x: x % 2 == 0, nums)

# Step 2: Square them
squared = map(lambda x: x**2, evens)

# Step 3: Sum all squared numbers
total = reduce(lambda x, y: x + y, squared)

print(total)  # Output: 56  (2^2 + 4^2 + 6^2)
```

---

## ⚠️ Common Mistakes

* Forgetting `from functools import reduce`
* Not converting `map()` or `filter()` to list to print
* Using complex logic inside lambda → reduce readability

---

## 📌 Exam-Ready Definitions

* **map()** → Applies a function to **all items** of an iterable
* **filter()** → Filters **items based on a condition**
* **reduce()** → Reduces an iterable to a **single value using a cumulative function**

---

## 🎯 Why This Topic Is Important

* Core for **functional programming in Python**
* Essential for **data processing, ML, and API development**
* Frequently asked in **BCA exams & Python interviews**

---

If you want next:
✅ **Practical problems combining map, filter, reduce**
✅ **Lambda + map/filter/reduce examples**
✅ **README.md formatted notes with diagrams**

Do you want me to **make a flow diagram showing map → filter → reduce workflow**?

# ## 🟢 Inner Functions in Python — **Detailed Explanation**

An **inner function** (also called a **nested function**) is a **function defined inside another function**.
Inner functions are used to **encapsulate functionality** and **create closures**.

---

## 📌 What is an Inner Function?

> An inner function is a function **defined inside another function** and can only be accessed **within the outer function**.

* Helps **hide functionality** from the outside
* Can **access variables** of the outer function

---

## 1️⃣ Syntax of an Inner Function

```python
def outer_function():
    # Outer function code
    def inner_function():
        # Inner function code
        pass
    # Call inner function
    inner_function()
```

---

## 2️⃣ Example: Basic Inner Function

```python
def outer():
    print("Outer function called")

    def inner():
        print("Inner function called")

    inner()  # Call inner function

outer()
```

**Output:**

```
Outer function called
Inner function called
```

**Explanation:**

* `inner()` is defined **inside `outer()`**
* Cannot be called outside `outer()`

---

## 3️⃣ Why Use Inner Functions?

1. **Encapsulation** – Hides the inner function from global scope
2. **Code organization** – Groups related functionality
3. **Closures** – Retain access to outer function variables
4. **Decorators** – Inner functions are used extensively

---

## 4️⃣ Inner Function Accessing Outer Variables

```python
def outer(name):
    def inner():
        print("Hello", name)
    inner()

outer("Amit")
```

**Output:**

```
Hello Amit
```

**Explanation:**

* `inner()` can **access variables** of `outer()`
* Useful for **closure and dynamic function behavior**

---

## 5️⃣ Returning Inner Function (Closure)

```python
def outer(x):
    def inner(y):
        return x + y
    return inner

add_five = outer(5)
print(add_five(10))  # Output: 15
```

**Explanation:**

* `outer(5)` returns `inner` function
* `inner` remembers `x = 5` → this is called a **closure**

---

## 6️⃣ Practical Example: Decorator Concept

```python
def decorator(func):
    def wrapper():
        print("Before function call")
        func()
        print("After function call")
    return wrapper

def say_hello():
    print("Hello!")

decorated = decorator(say_hello)
decorated()
```

**Output:**

```
Before function call
Hello!
After function call
```

**Explanation:**

* `wrapper()` is an inner function
* Allows **pre- and post-processing** around `say_hello()`

---

## 7️⃣ Key Points About Inner Functions

* Can **access outer function variables** (closure)
* **Not accessible** from outside the outer function unless returned
* Useful for **encapsulation, closures, and decorators**
* Can be **used as factory functions**

---

## 8️⃣ Difference Between Normal and Inner Function

| Feature  | Normal Function      | Inner Function                    |
| -------- | -------------------- | --------------------------------- |
| Scope    | Global / Local       | Only inside outer function        |
| Access   | Anywhere (if global) | Only within outer function        |
| Use Case | General purpose      | Encapsulation, closure, decorator |

---

## ⚠️ Common Mistakes

* Calling inner function **outside** the outer function → ❌ Error
* Forgetting to return inner function when creating **closure**
* Using complex logic inside inner functions → reduces readability

---

## 📌 Exam-Ready Definition

> An inner function in Python is a function **defined inside another function**, which can access the variables of the outer function and is used for **encapsulation, closure, and modularity**.

---

## 📝 Short Example for Exams

```python
def outer(x):
    def inner(y):
        return x + y
    return inner

add_five = outer(5)
print(add_five(10))  # Output: 15
```

---

## 🎯 Why This Topic Is Important

* Core concept for **closures and decorators**
* Used in **functional programming**
* Important for **modular and encapsulated code**
* Frequently asked in **BCA exams & Python interviews**

---

If you want next:
✅ **Closures in Python explained**
✅ **Decorators using inner functions**
✅ **README.md formatted notes with diagrams**

Do you want me to make **a full visual diagram showing inner function, closure, and decorator flow**?

# ## 🎨 Decorators in Python — **Detailed Explanation**

A **decorator** in Python is a **function that modifies another function** (or method) **without changing its source code**.
Decorators are widely used for **logging, authentication, timing, memoization, and access control**.

---

## 📌 What is a Decorator?

> A decorator is a **higher-order function** that takes a function as input and returns a **modified or enhanced function**.

* Enhances or extends functionality **dynamically**
* Keeps **code clean and DRY** (Don’t Repeat Yourself)

---

## 1️⃣ Syntax of a Decorator

```python
def decorator(func):
    def wrapper():
        # Code before function call
        func()
        # Code after function call
    return wrapper
```

* `func` → original function
* `wrapper()` → enhanced function
* Return `wrapper` function

---

## 2️⃣ Using a Decorator

```python
def decorator(func):
    def wrapper():
        print("Before function call")
        func()
        print("After function call")
    return wrapper

def say_hello():
    print("Hello!")

say_hello = decorator(say_hello)  # Decorating the function
say_hello()
```

**Output:**

```
Before function call
Hello!
After function call
```

---

## 3️⃣ Using `@` Syntax (Pythonic Way)

```python
def decorator(func):
    def wrapper():
        print("Before function call")
        func()
        print("After function call")
    return wrapper

@decorator
def say_hello():
    print("Hello!")

say_hello()
```

**Explanation:**

* `@decorator` is equivalent to:
  `say_hello = decorator(say_hello)`
* Cleaner and widely used in Python frameworks

---

## 4️⃣ Decorator With Arguments

```python
def decorator(func):
    def wrapper(*args, **kwargs):
        print("Before call")
        result = func(*args, **kwargs)
        print("After call")
        return result
    return wrapper

@decorator
def add(a, b):
    return a + b

print(add(5, 3))
```

**Output:**

```
Before call
After call
8
```

**Explanation:**

* `*args` and `**kwargs` allow decorator to work with any function signature

---

## 5️⃣ Multiple Decorators

```python
def deco1(func):
    def wrapper():
        print("Deco1 Before")
        func()
        print("Deco1 After")
    return wrapper

def deco2(func):
    def wrapper():
        print("Deco2 Before")
        func()
        print("Deco2 After")
    return wrapper

@deco1
@deco2
def greet():
    print("Hello!")

greet()
```

**Output:**

```
Deco1 Before
Deco2 Before
Hello!
Deco2 After
Deco1 After
```

**Explanation:**

* Decorators are applied **inside-out**: `greet = deco1(deco2(greet))`

---

## 6️⃣ Decorators With Return Values

```python
def decorator(func):
    def wrapper(*args, **kwargs):
        result = func(*args, **kwargs)
        return result * 2
    return wrapper

@decorator
def add(a, b):
    return a + b

print(add(5, 3))  # Output: 16
```

---

## 7️⃣ Real-World Examples

### 🔹 Logging Decorator

```python
def log(func):
    def wrapper(*args, **kwargs):
        print(f"Function {func.__name__} called with {args} and {kwargs}")
        return func(*args, **kwargs)
    return wrapper

@log
def multiply(a, b):
    return a * b

print(multiply(5, 4))
```

### 🔹 Timing Decorator

```python
import time

def timer(func):
    def wrapper(*args, **kwargs):
        start = time.time()
        result = func(*args, **kwargs)
        end = time.time()
        print(f"Execution time: {end - start} seconds")
        return result
    return wrapper

@timer
def compute():
    sum(range(1000000))

compute()
```

---

## 8️⃣ Key Points About Decorators

* Decorators are **higher-order functions**
* Can be applied with `@` syntax
* Can handle **any number of arguments** using `*args` and `**kwargs`
* Useful for **cross-cutting concerns** like logging, authentication, timing
* Can **stack multiple decorators**

---

## 9️⃣ Decorator vs Wrapper

| Feature    | Wrapper Function                | Decorator Function              |
| ---------- | ------------------------------- | ------------------------------- |
| Definition | Inner function inside decorator | Function that returns a wrapper |
| Purpose    | Enhances original function      | Returns enhanced function       |
| Example    | `wrapper()`                     | `decorator(func)`               |

---

## 10️⃣ Exam-Ready Definition

> A decorator in Python is a function that takes another function as input, adds functionality to it, and returns the enhanced function. Decorators are used with the `@` syntax for cleaner and reusable code.

---

## 📝 Short Example for Exams

```python
def decorator(func):
    def wrapper():
        print("Before call")
        func()
        print("After call")
    return wrapper

@decorator
def greet():
    print("Hello!")

greet()
```

Output:

```
Before call
Hello!
After call
```

---

## 🎯 Why This Topic Is Important

* Core concept for **Python OOP and functional programming**
* Used extensively in **Flask, Django, and API development**
* Essential for **BCA exams & Python interviews**
* Basis for **advanced topics** like **memoization and access control**

---

If you want next:
✅ **Closures vs Decorators explained visually**
✅ **Practical decorator examples with arguments**
✅ **README.md formatted notes with diagrams**

Do you want me to **make a full visual diagram showing decorators, inner functions, and closures together**?

Sure! Let’s go **step by step** to understand **Exception Handling in Python** clearly.

---

### **1. What is an Exception?**

An **exception** is an **error that occurs during the execution of a program**. It interrupts the normal flow of the program.

**Example of exceptions:**

```python
print(10 / 0)      # ZeroDivisionError
print(x)           # NameError, if x is not defined
```

Without handling, these errors will **terminate your program**.

---

### **2. Why Exception Handling?**

* To **prevent the program from crashing**.
* To **handle errors gracefully**.
* To allow the program to **take corrective actions**.

---

### **3. Basic Syntax of Exception Handling**

Python provides the **`try`, `except`, `else`, `finally`** blocks for exception handling:

```python
try:
    # Code that may raise an exception
except ExceptionType:
    # Code to handle the exception
else:
    # Code to run if no exception occurs
finally:
    # Code that always runs (optional)
```

---

### **4. Example of try-except**

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Invalid input! Please enter a number.")
else:
    print("Result is:", result)
finally:
    print("Execution completed.")
```

**Explanation:**

1. `try` → Code that may raise an exception.
2. `except` → Catches specific exceptions.
3. `else` → Runs only if no exception occurred.
4. `finally` → Always executes, used for cleanup (like closing files).

---

### **5. Catching Multiple Exceptions**

```python
try:
    x = int(input("Enter a number: "))
    y = 10 / x
except (ValueError, ZeroDivisionError) as e:
    print("Error occurred:", e)
```

Here, both `ValueError` and `ZeroDivisionError` are handled together.

---

### **6. Raising Exceptions Manually**

You can **raise an exception** using `raise`:

```python
age = int(input("Enter your age: "))
if age < 18:
    raise ValueError("Age must be at least 18")
```

---

### **7. Common Python Exceptions**

| Exception Type      | When it occurs                                       |
| ------------------- | ---------------------------------------------------- |
| `ZeroDivisionError` | Division by zero                                     |
| `ValueError`        | Invalid value input (e.g., converting string to int) |
| `TypeError`         | Wrong type operation (e.g., adding int + str)        |
| `FileNotFoundError` | File doesn’t exist                                   |
| `IndexError`        | Accessing invalid list index                         |
| `KeyError`          | Key not found in dictionary                          |

---

✅ **Summary:**

* Use `try` to wrap risky code.
* Use `except` to handle exceptions.
* Use `else` for normal execution if no exception occurs.
* Use `finally` to execute code always (cleanup).
* You can **catch multiple exceptions** and even **raise exceptions manually**.

---

If you want, I can also make a **diagram showing the flow of exception handling in Python**. It makes understanding way easier.

Do you want me to do that?

Sure! Let’s go **deeply into Python’s built-in exceptions**. Python provides **many built-in exceptions** to indicate different types of errors. Handling them properly helps make your program robust.

---

## **1. What are Built-in Exceptions?**

Built-in exceptions are **predefined error classes** in Python. When an error occurs, Python raises one of these exceptions automatically.

---

## **2. Common Built-in Exceptions**

Here’s a list of the most frequently used exceptions:

| **Exception**                         | **Description**                            | **Example**                              |
| ------------------------------------- | ------------------------------------------ | ---------------------------------------- |
| `ZeroDivisionError`                   | Division by zero                           | `10 / 0`                                 |
| `ValueError`                          | Invalid value for a function or operation  | `int("abc")`                             |
| `TypeError`                           | Operation applied to an inappropriate type | `"2" + 2`                                |
| `NameError`                           | Variable not defined                       | `print(x)` (if x is not defined)         |
| `IndexError`                          | Index out of range in a list, tuple, etc.  | `lst = [1,2]; lst[5]`                    |
| `KeyError`                            | Key not found in a dictionary              | `d = {"a":1}; d["b"]`                    |
| `AttributeError`                      | Invalid attribute reference                | `"abc".push(1)`                          |
| `FileNotFoundError`                   | File does not exist                        | `open("file.txt")` (if it doesn’t exist) |
| `ImportError` / `ModuleNotFoundError` | Cannot import a module                     | `import math2`                           |
| `OverflowError`                       | Number too large to handle                 | `2.0**10000`                             |
| `MemoryError`                         | Not enough memory                          | Allocating huge list                     |
| `StopIteration`                       | No more items in iterator                  | Using `next()` on exhausted iterator     |
| `IndentationError`                    | Wrong indentation                          | Code with wrong spaces/tabs              |
| `RuntimeError`                        | Generic runtime error                      | Miscellaneous runtime issues             |
| `KeyboardInterrupt`                   | Program interrupted by user                | Pressing Ctrl+C                          |

---

## **3. Example: Handling Built-in Exceptions**

```python
try:
    x = int(input("Enter a number: "))
    y = 10 / x
    lst = [1, 2, 3]
    print(lst[5])
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Invalid input!")
except IndexError:
    print("Index out of range!")
finally:
    print("Program ended.")
```

**Explanation:**

* Python raises different exceptions depending on the error.
* We can catch them individually to handle **specific errors**.
* `finally` always runs for cleanup.

---

## **4. Catch All Exceptions (Not Recommended Usually)**

```python
try:
    x = int(input("Enter a number: "))
    y = 10 / x
except Exception as e:
    print("An error occurred:", e)
```

* `Exception` is the **base class for most built-in exceptions**.
* This will catch **any exception**, but it’s better to handle specific ones.

---

### ✅ Summary:

* Built-in exceptions are predefined error classes in Python.
* Using `try-except`, you can handle them to avoid program crashes.
* Catch specific exceptions whenever possible for clarity.
* Use `Exception` as a last resort to catch all errors.

---

If you want, I can make a **table of all Python built-in exceptions with examples for each**—it’s like a ready reference for your coding exams or interviews.

Do you want me to do that?

Sure! Let’s dive into **User-Defined Exceptions in Python** in a clear, step-by-step way.

---

## **1. What is a User-Defined Exception?**

A **user-defined exception** is an **exception created by the programmer** to handle specific errors that are not covered by Python’s built-in exceptions.

* Useful when you want to enforce **custom rules** in your program.
* All user-defined exceptions **must inherit from the `Exception` class** (or its subclasses).

---

## **2. Syntax of User-Defined Exception**

```python
class MyCustomError(Exception):
    def __init__(self, message):
        self.message = message
        super().__init__(self.message)
```

* `MyCustomError` → Name of the exception
* `Exception` → Base class
* `message` → Optional custom message

---

## **3. Raising a User-Defined Exception**

```python
def check_age(age):
    if age < 18:
        raise MyCustomError("Age must be at least 18")
    else:
        print("Access granted")

try:
    age = int(input("Enter your age: "))
    check_age(age)
except MyCustomError as e:
    print("Error:", e)
```

**Explanation:**

1. `raise MyCustomError("message")` → Throws the exception.
2. `except MyCustomError as e:` → Catches the exception.
3. Prints the **custom error message**.

---

## **4. Why Use User-Defined Exceptions?**

* To enforce **custom validation rules**.
* To make your code **more readable** and **maintainable**.
* To handle **special cases** that built-in exceptions don’t cover.

**Example: Bank Account Withdrawal**

```python
class InsufficientFunds(Exception):
    pass

def withdraw(balance, amount):
    if amount > balance:
        raise InsufficientFunds("Not enough balance!")
    return balance - amount

try:
    balance = 5000
    balance = withdraw(balance, 6000)
except InsufficientFunds as e:
    print(e)
```

Output:

```
Not enough balance!
```

---

### ✅ **Summary**

1. User-defined exceptions are **custom errors** created by the programmer.
2. They **inherit from the `Exception` class**.
3. Use `raise` to trigger the exception.
4. Use `try-except` to **catch and handle** it.
5. They are useful for **specific business rules** and validations.

---

