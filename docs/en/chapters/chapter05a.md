# **Unit 5a: Flow of Control and Functions**

---

## **Introduction**

When writing programs, the order in which instructions are executed is crucial. In Python, we control the flow of execution using **control structures** like sequence, selection, and repetition. We also use **functions** to make our code modular and reusable. In this unit, we’ll explore how these control structures work and how to write and use functions in Python. By the end of this unit, you’ll be able to write more efficient and well-structured code.

---

## **5a.1 Control Structures**

**Control Structures** are the fundamental building blocks that determine the flow of execution in a program. Python uses three main control structures:

---

### **1. Sequence**

In a **sequence**, statements are executed one after the other in the order they appear. This is the simplest form of control flow where each line of code runs sequentially.

**Example**:
```python
print("Step 1")
print("Step 2")
print("Step 3")
```

In the above example, the steps are executed in sequence, one after the other.

---

### **2. Selection (Decision)**

**Selection** allows the program to take different paths based on certain conditions. In Python, selection is handled using conditional statements such as `if`, `if-else`, and `elif`.

- **if Statement**: Executes a block of code if a condition is true.

    **Example**:  
    ```python  
    if age >= 18:  
      print("You are an adult")  
    ```  

- **if-else Statement**: Executes one block of code if the condition is true and another block if it is false.

    **Example**:  
    ```python  
    if age >= 18:  
      print("Adult")  
    else:  
      print("Not an adult")  
    ```  

- **Nested if Statement**: Multiple `if` statements inside one another. This allows checking multiple conditions.

    **Example**:  
    ```python  
    if age >= 18:  
      if age >= 65:  
         print("Senior Citizen")  
      else:  
         print("Adult")  
    ```  

---

### **3. Repetition (Iteration)**

**Repetition** allows a block of code to be executed repeatedly as long as a condition is met. Python uses loops for repetition: **for loops** and **while loops**.

- **for Loop**: Repeats a block of code a specific number of times, usually iterating over a sequence like a list or a range of numbers.

    **Example**:  
    ```python  
    for i in range(5):  
      print(i)  
    ```  

    This loop will print the numbers 0 to 4.  

- **while Loop**: Repeats a block of code as long as the condition is true.

    **Example**:  
    ```python  
    i = 0  
    while i < 5:  
      print(i)  
      i += 1  
    ```  

    This loop will print the numbers 0 to 4, similar to the `for` loop.  

- **break Statement**: Exits the loop prematurely before all iterations are completed.

    **Example**:  
    ```python  
    for i in range(5):  
      if i == 3:  
         break  
      print(i)  
    ```  

    This will print 0, 1, 2 and then stop when `i` equals 3.  

- **continue Statement**: Skips the rest of the code in the current iteration and moves to the next iteration.

    **Example**:  
    ```python  
    for i in range(5):  
      if i == 3:  
         continue  
      print(i)  
    ```  

    This will print 0, 1, 2, 4, skipping 3.  

---

## **5a.2 Functions**

**Functions** are blocks of reusable code designed to perform a specific task. Functions help you avoid writing repetitive code and make your programs easier to understand and maintain.

---

### **Why Do We Need Functions?**

Functions allow us to:
1. Break down large problems into smaller, manageable tasks.
2. Avoid repeating the same code in different parts of a program.
3. Improve code organization, readability, and modularity.

---

### **Types of Functions**

1. **Built-in Functions**: Python has many built-in functions such as `print()`, `len()`, and `sum()`. These are predefined functions that you can use directly without having to define them.

    **Example**:  
    ```python  
    print(len("Hello"))  # Outputs 5  
    ```  

2. **User-defined Functions**: These are functions created by the user to perform specific tasks. You define a function using the `def` keyword.

    **Example**:  
    ```python  
    def greet(name):  
      print(f"Hello, {name}!")  

    greet("Alice")  # Outputs: Hello, Alice!  
    ```  

---

### **Structure of a Function**

A Python function follows a specific structure:

1. **Function Definition**: This is where the function is created. It starts with the `def` keyword, followed by the function name, parentheses, and a colon. The body of the function is indented.

    **Example**:  
    ```python  
    def function_name(parameters):  
      # function body  
    ```  

2. **Function Call**: To execute the function, you call it by its name and pass any required arguments.

    **Example**:  
    ```python  
    function_name(arguments)  
    ```  

---

### **Example of a User-Defined Function**

Here’s an example of a function that adds two numbers and returns the result:

```python
def add_numbers(a, b):
     return a + b  

result = add_numbers(5, 3)
print(result)  # Outputs: 8
```

---

### **Function Parameters and Return Values**

- **Parameters**: Functions can take parameters (inputs) to perform operations based on those inputs. Parameters are specified within the parentheses of the function definition.

- **Return Values**: Functions can return a result using the `return` statement. The result can be assigned to a variable when the function is called.

---

## **Important Terminology**

- **Sequence**: The execution of instructions in a specific order, one after another.
- **Selection**: A control structure that allows the program to choose between different paths based on conditions (e.g., if, if-else, nested if).
- **Repetition**: A control structure that allows the repeated execution of a block of code (e.g., for, while).
- **Iteration**: Repeating a block of code using loops like `for` and `while`.
- **If Statement**: A conditional statement that executes a block of code if a condition is true.
- **If-Else Statement**: A conditional statement that chooses between two blocks of code based on whether a condition is true or false.
- **For Statement**: A loop that repeats a block of code a specific number of times.
- **While Statement**: A loop that repeats a block of code as long as a condition is true.
- **Break Statement**: Exits a loop before it has completed all iterations.
- **Continue Statement**: Skips the current iteration of a loop and moves to the next iteration.
- **Functions**: Blocks of reusable code designed to perform specific tasks.
- **User-Defined Functions**: Functions created by the programmer.
- **Built-in Functions**: Predefined functions that come with Python.

---

## **Quiz**

1. Which control structure allows for executing code in a specific order?  
    a) Sequence  
    b) Selection  
    c) Iteration  
    d) Function  

2. What type of statement is used to choose between two possible outcomes based on a condition?  
    a) for loop  
    b) if-else statement  
    c) while loop  
    d) break statement  

3. True or False: A `for` loop repeats a block of code indefinitely as long as the condition is true.  

4. What does the `break` statement do in a loop?  
    a) Repeats the loop  
    b) Skips the current iteration  
    c) Exits the loop  
    d) Pauses the loop  

5. Which of the following is an example of a built-in function in Python?  
    a) print()  
    b) greet()  
    c) sum_numbers()  
    d) calculate_sum()  

6. True or False: Functions in Python are used to organize code and make it reusable.  

7. How do you define a user-defined function in Python?  
    a) Use the `def` keyword  
    b) Use the `function` keyword  
    c) Use the `for` keyword  
    d) Use the `loop` keyword  

8. What type of loop is used when you know exactly how many times you want to repeat a block of code?  
    a) while loop  
    b) if-else statement  
    c) for loop  
    d) break statement  

9. What is the purpose of the `continue` statement?  
    a) Exit the loop  
    b) Skip the rest of the current iteration and move to the next one  
    c) Repeat the loop indefinitely  
    d) Stop the execution of the program  

10. True or False: User-defined functions must always return a value.  

---

## **Answers**

1. a) Sequence
2. b) if-else statement
3. False
4. c) Exits the loop
5. a) print()
6. True
7. a) Use the `def` keyword
8. c) for loop
9. b) Skip the rest of of the current iteration and move to the next one
10. False

---
