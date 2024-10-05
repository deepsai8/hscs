# **Unit 5: Getting Started with Python**

---

## **Introduction:**

Python is a popular, easy-to-learn programming language that is widely used in web development, data science, artificial intelligence, and more. In this unit, we’ll explore the basics of Python programming, from understanding the structure of a program to working with variables, operators, and data types. By the end of this unit, you’ll have the foundational skills to start writing your own Python programs!

---

## **5.1 Introduction to Python**

**What is Python?**
Python is a high-level, interpreted programming language known for its simplicity and readability. It allows developers to write programs with fewer lines of code compared to other programming languages like C++ or Java.

**Features of Python**:
- **Easy to Learn and Use**: Python’s syntax is simple and clear, making it ideal for beginners.
- **Interpreted**: Python programs are executed line by line, making it easy to test and debug.
- **Cross-Platform**: Python works on different operating systems like Windows, macOS, and Linux.
- **Extensive Libraries**: Python has a rich collection of libraries that make tasks like data manipulation, web development, and machine learning much easier.

**Interactive Mode vs. Script Mode**:
- **Interactive Mode**: You can type Python code directly into the Python interpreter and get immediate results. It’s great for testing small code snippets.
- **Script Mode**: You can write your code in a file (called a script) and run the entire program at once. This is useful for larger programs.

---

## **5.2 Structure of a Python Program**

A Python program typically follows a simple structure:

1. **Comments**: These are non-executable lines that help explain what the code does. In Python, comments start with `#`.
    ```python  
    # This is a comment  
    ```  
2. **Statements**: Each line of code is a statement. A statement is an instruction for the computer to execute.
    ```python  
    print("Hello, World!")  
    ```  
3. **Indentation**: Python uses indentation (spaces or tabs) to define blocks of code, such as the body of loops or functions. Unlike other languages, Python does not use curly braces (`{}`).
    ```python  
    if age >= 18:  
     print("You are an adult")  
    ```  

---

## **5.3 Identifiers, Keywords, Constants, and Variables**

### **Identifiers**:
Identifiers are names given to variables, functions, or other entities in a program. They must start with a letter (A-Z or a-z) or an underscore (`_`) and can be followed by letters, digits (0-9), or underscores. Identifiers are case-sensitive.

**Example:**
```python
my_variable = 10
Age = 25
```

### **Keywords**:
Keywords are reserved words in Python that have special meaning and cannot be used as identifiers. Some examples of Python keywords are `if`, `else`, `while`, `for`, `def`, `return`.

**Example:**
```python
if age > 18:
     print("Eligible")  
```

### **Constants**:
Constants are values that do not change during the execution of a program. Python doesn’t have a strict constant declaration, but by convention, variables that should not be changed are written in all uppercase letters.

**Example:**
```python
PI = 3.14
MAX_SIZE = 100
```

### **Variables**:
A **variable** is a named storage location that holds a value, which can change during the execution of the program. Variables are assigned using the `=` operator.

**Example:**
```python
name = "Alice"
age = 20
```

---

## **5.4 Types of Operators**

Python has several types of operators that perform different operations on variables and values.

1. **Arithmetic Operators**:
    Used for basic mathematical operations.  
    - `+` (Addition), `-` (Subtraction), `*` (Multiplication), `/` (Division), `//` (Floor Division), `%` (Modulus), `**` (Exponentiation)  

    **Example:**  
    ```python  
    result = 10 + 5  # Adds 10 and 5  
    ```  

2. **Comparison Operators**:
    Used to compare two values.  
    - `==` (Equal to), `!=` (Not equal to), `>` (Greater than), `<` (Less than), `>=` (Greater than or equal to), `<=` (Less than or equal to)  

    **Example:**  
    ```python  
    if 10 > 5:  
     print("True")  
    ```  

3. **Logical Operators**:
    Used to combine conditional statements.  
    - `and`, `or`, `not`  

    **Example:**  
    ```python  
    if age > 18 and age < 60:  
     print("Eligible")  
    ```  

4. **Assignment Operators**:
    Used to assign values to variables.  
    - `=`, `+=`, `-=`, `*=`, `/=`, etc.  

    **Example:**  
    ```python  
    x = 10  
    x += 5  # Equivalent to x = x + 5  
    ```  

---

## **5.5 Precedence of Operators**

**Operator precedence** determines the order in which operations are performed in an expression. For example, multiplication and division have a higher precedence than addition and subtraction.

**Example:**
```python
result = 2 + 3 * 4  # Multiplication happens first, so result is 14
```

To change the order of operations, you can use parentheses:
```python
result = (2 + 3) * 4  # Now addition happens first, so result is 20
```

---

## **5.6 Data Types**

Python supports various built-in data types:

1. **int**: Whole numbers (e.g., 10, -5).
2. **float**: Numbers with decimals (e.g., 3.14, -2.5).
3. **str**: Strings (text enclosed in quotes) (e.g., "Hello").
4. **bool**: Boolean values (`True` or `False`).
5. **list**: An ordered collection of values (e.g., `[1, 2, 3]`).
6. **tuple**: Similar to a list, but immutable (e.g., `(1, 2, 3)`).
7. **dict**: A collection of key-value pairs (e.g., `{"name": "Alice", "age": 25}`).

**Example:**
```python
age = 25  # int
pi = 3.14  # float
name = "John"  # str
is_adult = True  # bool
```

---

## **5.7 Statements, Expressions, and Comments**

### **Statements**:
A statement is a line of code that performs a specific action.

**Example:**
```python
print("Hello, World!")  # This is a statement
```

### **Expressions**:
An expression is a combination of variables, operators, and values that returns a result.

**Example:**
```python
result = 10 + 5  # This is an expression
```

### **Comments**:
Comments are non-executable lines in the code that explain what the code does. They are created using the `#` symbol.

**Example:**
```python
# This is a comment
print("Hello!")  # This prints Hello!
```

---

## **5.8 Input and Output Statements**

### **Input**:
The `input()` function allows the user to input data during the program execution.

**Example:**
```python
name = input("Enter your name: ")
print("Hello, " + name)
```

### **Output**:
The `print()` function is used to display output.

**Example:**
```python
age = 20
print("This is an output statement")
print("Your age: ", age)
```

---

## **5.9 Data Type Conversion**

Python allows you to convert one data type to another. This is known as **type conversion**.

### **Implicit Conversion**:
Python automatically converts data types when needed.

**Example:**
```python
x = 10  # int  
y = 10.5 # float
z = x + y  # z will automatically be a float (20.5)
```

### **Explicit Conversion**:
You can manually convert data types using functions like `int()`, `float()`, and `str()`.

**Example:**
```python
x = "100"
y = int(x)  # Converts the string "100" into an integer 100
```

---

## **5.10 Debugging**

**Debugging** is the process of finding and fixing errors (bugs) in your code. Python provides error messages that help locate problems, and tools like **IDEs** (Integrated Development Environments) allow you to step through the code and observe its behavior to find and fix issues.

---

## **Important Terminology:**

- **Interpreter**: A program that executes code line by line.
- **Identifiers**: Names given to variables, functions, etc.
- **Keywords**: Reserved words in Python that cannot be used as identifiers (e.g., `if`, `else`).
- **Constants**: Values that don’t change during program execution.
- **Variables**: Named locations that store data values.
- **Operators**: Symbols that perform operations (e.g., `+`, `*`).
- **Data Types**: Different types of data (e.g

., `int`, `str`, `float`).
- **Expressions**: Combinations of variables, values, and operators that produce a result.
- **Comments**: Non-executable lines of text in code that explain what the code does.
- **Conversion**: Changing data from one type to another.

---

## **Quiz**

1. What does an interpreter do?  
    a) Converts Python code into machine language  
    b) Executes Python code line by line  
    c) Compiles Python code into binary  
    d) Checks Python code for errors  

2. True or False: Identifiers can start with numbers in Python.  

3. Which of the following is NOT a Python keyword?  
    a) for  
    b) return  
    c) while  
    d) print  

4. Which operator is used to multiply two numbers in Python?  
    a) +  
    b) *  
    c) /  
    d) %  

5. True or False: The `input()` function in Python is used to display output to the user.  

6. Which data type represents a sequence of characters in Python?  
    a) int  
    b) float  
    c) str  
    d) bool  

7. What symbol is used to create comments in Python?  
    a) `//`  
    b) `#`  
    c) `/* */`  
    d) `""" """`  

8. True or False: Python automatically converts an integer to a float when needed.  

9. Which of the following is an example of an expression in Python?  
    a) print("Hello, World!")  
    b) x = 10 + 5  
    c) # This is a comment  
    d) input("Enter your name")  

10. What is debugging?  
    a) Writing code  
    b) Testing code  
    c) Finding and fixing errors in code  
    d) Documenting code  

---

## **Answers**

1. b) Executes Python code line by line
2. False
3. d) print
4. b) *
5. False
6. c) str
7. b) `#`
8. True
9. b) x = 10 + 5
10. c) Finding and fixing errors in code

---

This unit has introduced you to the basics of Python programming, from understanding the structure of a program to working with variables, operators, and data types. You’re now ready to start coding and exploring the endless possibilities of Python!

---