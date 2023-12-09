# UBPy Language Specification

UBPy is a programming language inspired by Python.

## 1. Data Types

UBPy supports the following basic data types:

- `Integer`: Representing whole numbers.
- `Floating-point numbers`: Representing values in decimals.
- `Text`: Representing a sequence of characters.
- `Boolean values`: Representing True or False values.
- `List`: An ordered collection of elements.
- `Map`: A collection of key-value pairs.

### Keywords

| Data Type | Keyword  | Input Syntax        | Example                                    |
|-----------|----------|---------------------|--------------------------------------------|
| Integer   | int      | int A = 1           | A = 1                                      |
| Float     | flt      | flt A = 1.1         | A = 1.1                                    |
| Text      | text     | text A = 'apple'    | A = 'apple'                                |
| Boolean   | logic    | logic True, False    | True, False                                |
| List      | list_of  | My_list[] = list_of [] | My_list = []                               |
| Map       | dict_of  | My_dict = dict_of {'country': 'Pakistan', 'Australia'} | My_dict = {'country': 'Pakistan', 'Australia'} |

List and maps are both data structures and data types in UBPy.

## 2. Identifier Syntax

An identifier in UBPy is a name used to identify a variable, function, class, or other objects. Identifiers:

- Must start with a letter (a-z, A-Z).
- Can be followed by letters, digits (0-9), or underscores.
- Must not be the same as any default keywords within the language.
- Are case-sensitive.

## 3. Return Types

UBPy functions can return values of types integers, floating-point numbers, text (strings), and logic (boolean values).

### Examples

- Integer: `bring_back 42`
- Float: `bring_back 3.14`
- Text: `bring_back "Hello, world!"`
- Logic: `bring_back True` / `bring_back False`

## 4. Relevant Punctuators

- `:`: Colon, used in control flow statements and function/class definitions.
- `,`: Comma, used to separate elements in data structures and function arguments.
- `.`: Dot, used for attribute and method access.
- `()`: Parentheses, used for function/method calls and defining tuples.
- `[]`: Square brackets, used for creating lists and accessing elements.
- `{}`: Curly braces, used for creating dictionaries (maps) and defining code blocks.
- `#`: Hash, used for commenting.

## 5. Operators

UBPy supports various operators, including arithmetic, comparison, logical, assignment, and other operators.

### Examples

```ubpy
# Arithmetic operators
result = 10 + 5
result = 10 - 5
result = 10 * 5
result = 10 / 5
result = 10 % 3
result = 2 ** 3

# Comparison operators
if x == y:
if x != y:
if x > y:
if x < y:
if x >= y:
if x <= y:

# Logical operators
if x > 0 and y > 0:
if x > 0 or y > 0:
if not x > 0:

# Assignment operators
x = 10
x += 5  # equivalent to x = x + 5
x -= 5  # equivalent to x = x - 5

```

## 6. Control Flow Keywords
## In Python
if
else
elif
while
for
break
continue

## In UBPy
given
otherwise
else_if
while_so
for_each
stop
go_on

## Conditional Statements
The given, otherwise, and else_if keywords are used for conditional branching:

int x = 10
given x > 5:
    display("x is greater than 5")
else_if x == 5:
    display("x is equal to 5")
otherwise:
    display("x is less than 5")

## Loops
UBPy supports while_so and for_each loops:

# Example using while_so loop
int count = 0
while_so count < 5:
    display(count)
    count += 1

# Example using for_each loop
fruits[3] = list_of ['apple', 'banana', 'cherry']
for_each fruit in fruits:
    display(fruit)

## 7. Function Keywords

| Keyword       | Description                                | Python Equivalent |
|---------------|--------------------------------------------|-------------------|
| `doing`       | Used to define a function/method           | `def`             |
| `bring_back`  | Used to specify the return value of a function | `return`      |
| `display`     | Used to print output to the console        | `print`           |
| `take`        | Used to receive input from the user        | `input`           |

UBPy supports function overloading natively. You can define multiple methods with the same name but different parameter lists in a class, and UBPy will automatically handle function overloading based on the number and types of arguments passed during method calls.


## Function Definition
doing function_name(param1, param2, ...):

## Function Body
bring_back value_to_return

## 8. Other Keywords

| Keyword    | Description                                                  | Python Equivalent |
|------------|--------------------------------------------------------------|-------------------|
| `bring`    | Used to import modules or specific objects from modules into the current namespace | `import`          |
| `extract`  | Used to unpack data from lists into individual variables    | N/A               |
| `as`       | Used for aliasing, providing an alternate name for a module, class, or function | `as`              |

Examples:

# Aliasing a module in UBPy
bring math as my_math

# Unpacking a list in UBPy
my_list[3] = list_of [1, 2, 3]
text a, b, c = extract my_list

## 9. Classes and Object-Oriented Programming
UBPy fully supports inheritance, function overriding, encapsulation, and abstraction.

## Class Definition
classy ClassName:

# Inheritance

classy SubClass(is_a=BaseClass):

# Accessing Parent Class Attributes or Methods
base(attribute_name)
base(method_name(param1, param2, ...))

# Object Instantiation
obj = ClassName(arguments)

# Encapsulation
This is done by putting access modifiers before data type and identifier. Attributes or methods without an access modifier will be considered public and accessible through anywhere within the code.

# Function Overriding
Function overriding allows a subclass to provide a specific implementation for a method that is already defined in its parent class.






