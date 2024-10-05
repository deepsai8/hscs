# **Unit 7: Suggested Practical List**

---

## **Introduction**

This unit includes several practical Python programming exercises to help you strengthen your coding skills. Each exercise covers different concepts such as loops, conditionals, functions, and data structures. We will first present the skeletal code for each exercise, followed by the complete solution with explanations. After each exercise, you will find a set of quiz questions along with their answers to test your understanding of the concepts.

---

## **Skeletal Code for All Practical Projects**

1. **Print "Hello computer world!"**
   ```python
   # Skeleton
   # print("Hello computer world!")
   ```

2. **Add Two Numbers**
   ```python
   # Skeleton
   # num1 =
   # num2 =
   # result =
   # print(result)
   ```

3. **Print the Difference of Two Numbers**
   ```python
   # Skeleton
   # num1 =
   # num2 =
   # result =
   # print(result)
   ```

4. **Find the Larger of Two Numbers**
   ```python
   # Skeleton
   # num1 =
   # num2 =
   # if num1 > num2:
   #    print(num1)
   # else:
   #    print(num2)
   ```

5. **Find the Square Root**
   ```python
   # Skeleton
   # import math
   # num =
   # sqrt =
   # print(sqrt)
   ```

6. **Swap Two Variables**
   ```python
   # Skeleton
   # a =
   # b =
   # a, b = b, a
   # print(a, b)
   ```

7. **Convert Kilometers to Miles**
   ```python
   # Skeleton
   # km =
   # miles =
   # print(miles)
   ```

8. **Convert Celsius to Fahrenheit**
   ```python
   # Skeleton
   # celsius =
   # fahrenheit =
   # print(fahrenheit)
   ```

9. **Find LCM**
   ```python
   # Skeleton
   # def find_lcm(x, y):
   #    # LCM logic here
   ```

10. **Find HCF**
    ```python
    # Skeleton
    # def find_hcf(x, y):
    #    # HCF logic here
    ```

11. **Print the First Ten Natural Numbers Using a While Loop**
    ```python
    # Skeleton
    # i = 1
    # while i <= 10:
    #    print(i)
    #    i += 1
    ```

12. **Print the Characters in the String 'PYTHON' Using a For Loop**
    ```python
    # Skeleton
    # for char in 'PYTHON':
    #    print(char)
    ```

13. **Print a Pattern for a Number Input by the User**
    ```python
    # Skeleton
    # num = int(input("Enter a number: "))
    # for i in range(1, num+1):
    #    # print pattern
    ```

14. **Find the Area and Perimeter of a Rectangle Using a User-Defined Function**
    ```python
    # Skeleton
    # def calculate_rectangle(length, breadth):
    #    # calculate area and perimeter
    ```

15. **Append Element in a List**
    ```python
    # Skeleton
    # my_list = []
    # element =
    # my_list.append(element)
    # print(my_list)
    ```

16. **Create a Dictionary**
    ```python
    # Skeleton
    # my_dict = {}
    # my_dict['key'] = 'value'
    # print(my_dict)
    ```

17. **Find the Factorial of a Number**
    ```python
    # Skeleton
    # def factorial(n):
    #    # factorial logic
    ```

---

## **Complete Solutions with Explanations**

### **1. Print "Hello computer world!"**

**Complete Code:**
```python
print("Hello computer world!")
```

**Explanation:**
This program prints the string "Hello computer world!" using Python's built-in `print()` function.

---

### **2. Add Two Numbers**

**Complete Code:**
```python
num1 = 5
num2 = 3
result = num1 + num2
print(result)
```

**Explanation:**
This program adds two numbers and prints the result.

---

### **3. Print the Difference of Two Numbers**

**Complete Code:**
```python
num1 = 10
num2 = 7
result = num1 - num2
print(result)
```

**Explanation:**
This program calculates the difference between two numbers and prints the result.

---

### **4. Find the Larger of Two Numbers**

**Complete Code:**
```python
num1 = 10
num2 = 15
if num1 > num2:
    print(num1)
else:
    print(num2)
```

**Explanation:**
This program compares two numbers and prints the larger one using an `if-else` statement.

---

### **5. Find the Square Root**

**Complete Code:**
```python
import math
num = 16
sqrt = math.sqrt(num)
print(sqrt)
```

**Explanation:**
This program uses Python's `math` module to calculate and print the square root of a number.

---

### **6. Swap Two Variables**

**Complete Code:**
```python
a = 5
b = 10
a, b = b, a
print(a, b)
```

**Explanation:**
This program swaps the values of two variables and prints the result.

---

### **7. Convert Kilometers to Miles**

**Complete Code:**
```python
km = 5
miles = km * 0.621371
print(miles)
```

**Explanation:**
This program converts kilometers to miles using the conversion factor `1 km = 0.621371 miles`.

---

### **8. Convert Celsius to Fahrenheit**

**Complete Code:**
```python
celsius = 25
fahrenheit = (celsius * 9/5) + 32
print(fahrenheit)
```

**Explanation:**
This program converts a temperature from Celsius to Fahrenheit using the formula `F = (C * 9/5) + 32`.

---

### **9. Find LCM**

**Complete Code:**
```python
def find_lcm(x, y):
    greater = max(x, y)
    while True:
        if greater % x == 0 and greater % y == 0:
            lcm = greater
            break
        greater += 1
    return lcm

print(find_lcm(4, 6))
```

**Explanation:**
This program finds the least common multiple (LCM) of two numbers.

---

### **10. Find HCF**

**Complete Code:**
```python
def find_hcf(x, y):
    smaller = min(x, y)
    for i in range(1, smaller + 1):
        if x % i == 0 and y % i == 0:
            hcf = i
    return hcf

print(find_hcf(4, 6))
```

**Explanation:**
This program finds the highest common factor (HCF) of two numbers.

---

### **11. Print the First Ten Natural Numbers Using a While Loop**

**Complete Code:**
```python
i = 1
while i <= 10:
    print(i)
    i += 1
```

**Explanation:**
This program prints the first ten natural numbers using a `while` loop.

---

### **12. Print the Characters in the String 'PYTHON' Using a For Loop**

**Complete Code:**
```python
for char in 'PYTHON':
    print(char)
```

**Explanation:**
This program prints each character of the string "PYTHON" using a `for` loop.

---

### **13. Print a Pattern for a Number Input by the User**

**Complete Code:**
```python
num = int(input("Enter a number: "))
for i in range(1, num + 1):
    print('*' * i)
```

**Explanation:**
This program prints a pattern of stars based on the user input.

---

### **14. Find the Area and Perimeter of a Rectangle Using a User-Defined Function**

**Complete Code:**
```python
def calculate_rectangle(length, breadth):
    area = length * breadth
    perimeter = 2 * (length + breadth)
    return area, perimeter

length = 5
breadth = 3
area, perimeter = calculate_rectangle(length, breadth)
print("Area:", area)
print("Perimeter:", perimeter)
```

**Explanation:**
This program calculates the area and perimeter of a rectangle using a user-defined function.

---

### **15. Append Element in a List**

**Complete Code:**
```python
my_list = [1, 2, 3]
element = 4
my_list.append(element)
print(my_list)
```

**Explanation:**
This program appends an element to a list using the `append()` method.

---

### **16. Create a Dictionary**

**Complete Code:**
```python
my_dict = {}
my_dict['name'] = 'Alice'
my_dict['age'] = 25
print(my_dict)
```

**Explanation:**
This program creates a dictionary with key-value pairs.

---

### **17. Find the Factorial of a Number**

**Complete Code:**
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n

-1)

print(factorial(5))
```

**Explanation:**
This program calculates the factorial of a number using recursion.

---

## **Quiz for Each Practical Project**

Each practical project has its own set of quiz questions to test your understanding. Here are the quiz questions for each project:

---

### **Quiz 1: Print "Hello computer world!"**

1. What function is used to display output in Python?
2. How do you print text in Python?
3. What symbol is used to indicate a string in Python?
4. True or False: You need to import a library to use the `print()` function.
5. What will `print("Hello computer world!")` output?

---

### **Quiz 2: Add Two Numbers**

1. What operator is used to add two numbers in Python?
2. How do you assign a value to a variable in Python?
3. What will `print(5 + 3)` output?
4. True or False: Variables in Python must be declared with their data type.
5. What is the result of `num1 = 5` and `num2 = 7` followed by `print(num1 + num2)`?

---

### **Quiz 3: Print the Difference of Two Numbers**

1. What operator is used to subtract two numbers in Python?
2. What will `print(10 - 3)` output?
3. True or False: `10 - 5` is a valid Python expression.
4. If `num1 = 15` and `num2 = 5`, what will `print(num1 - num2)` output?
5. What is the result of `print(20 - 10)`?

---

### **Quiz 4: Find the Larger of Two Numbers**

1. What keyword is used to create a conditional statement in Python?
2. How do you compare two numbers to check if one is larger in Python?
3. True or False: The `else` block is required after an `if` statement.
4. What will the following code output:
   ```python
   if 10 > 5:
       print("Larger")
   else:
       print("Smaller")
   ```
5. What is the result of comparing `15 > 20`?

---

### **Quiz 5: Find the Square Root**

1. Which Python module is used to find the square root of a number?
2. What function is used to calculate the square root in Python?
3. True or False: The `sqrt()` function can only be used after importing the `math` module.
4. What will `math.sqrt(25)` return?
5. If `num = 36`, what will `math.sqrt(num)` return?

---

### **Quiz 6: Swap Two Variables**

1. How do you swap the values of two variables in Python?
2. What will `a, b = 10, 20` followed by `a, b = b, a` output for `a` and `b`?
3. True or False: The `swap` function is built into Python.
4. What does `a, b = b, a` do in Python?
5. What is the result of swapping `a = 5` and `b = 10`?

---

### **Quiz 7: Convert Kilometers to Miles**

1. What is the conversion factor from kilometers to miles?
2. How do you multiply two variables in Python?
3. What will `5 * 0.621371` output?
4. True or False: The `*` operator is used for multiplication in Python.
5. What is the result of converting 10 kilometers to miles?

---

### **Quiz 8: Convert Celsius to Fahrenheit**

1. What is the formula to convert Celsius to Fahrenheit?
2. What will the following code output:
   ```python
   celsius = 0
   fahrenheit = (celsius * 9/5) + 32
   print(fahrenheit)
   ```
3. True or False: `(32 * 9/5) + 32` will convert 32°C to Fahrenheit.
4. What is the result of converting 100°C to Fahrenheit?
5. What is the Fahrenheit equivalent of -40°C?

---

### **Quiz 9: Find LCM**

1. What does LCM stand for?
2. How do you find the LCM of two numbers in Python?
3. True or False: The LCM of 4 and 6 is 12.
4. What will `find_lcm(3, 5)` return?
5. What is the LCM of 8 and 12?

---

### **Quiz 10: Find HCF**

1. What does HCF stand for?
2. What is another name for HCF?
3. True or False: The HCF of 12 and 18 is 6.
4. What will `find_hcf(8, 12)` return?
5. What is the HCF of 15 and 20?

---

### **Quiz 11: Print the First Ten Natural Numbers Using a While Loop**

1. What is the syntax for a `while` loop in Python?
2. How do you increment a variable inside a `while` loop?
3. True or False: The condition in a `while` loop must always be `True` to run.
4. What will the following code output:
   ```python
   i = 1
   while i <= 3:
       print(i)
       i += 1
   ```
5. What are the first ten natural numbers?

---

### **Quiz 12: Print the Characters in the String 'PYTHON' Using a For Loop**

1. What is the syntax for a `for` loop in Python?
2. How do you iterate over each character in a string in Python?
3. True or False: The `for` loop is used to iterate over sequences in Python.
4. What will the following code output:
   ```python
   for char in 'PYTHON':
       print(char)
   ```
5. What are the characters in the string "PYTHON"?

---

### **Quiz 13: Print a Pattern for a Number Input by the User**

1. What function is used to take user input in Python?
2. How do you create a loop that runs `n` times in Python?
3. True or False: The `*` operator can be used to repeat strings in Python.
4. What will the following code output if the user inputs `3`?
   ```python
   num = 3
   for i in range(1, num + 1):
       print('*' * i)
   ```
5. What is the result of printing a pattern for the input `4`?

---

### **Quiz 14: Find the Area and Perimeter of a Rectangle Using a User-Defined Function**

1. How do you define a function in Python?
2. What is the formula for the area of a rectangle?
3. True or False: Functions in Python can return multiple values.
4. What will the following code output for length `5` and breadth `3`?
   ```python
   def calculate_rectangle(length, breadth):
       area = length * breadth
       perimeter = 2 * (length + breadth)
       return area, perimeter
   print(calculate_rectangle(5, 3))
   ```
5. What is the perimeter of a rectangle with length `10` and breadth `5`?

---

### **Quiz 15: Append Element in a List**

1. What method is used to add an element to the end of a list in Python?
2. How do you create an empty list in Python?
3. True or False: Lists in Python are mutable.
4. What will the following code output:
   ```python
   my_list = [1, 2, 3]
   my_list.append(4)
   print(my_list)
   ```
5. What is the result of appending `5` to the list `[10, 20]`?

---

### **Quiz 16: Create a Dictionary**

1. How do you create a dictionary in Python?
2. What data structure stores key-value pairs in Python?
3. True or False: Dictionary keys must be unique.
4. What will the following code output:
   ```python
   my_dict = {'name': 'Alice', 'age': 25}
   print(my_dict['name'])
   ```
5. How do you add a key-value pair to a dictionary?

---

### **Quiz 17: Find the Factorial of a Number**

1. What is the formula for calculating a factorial?
2. How do you define a recursive function in Python?
3. True or False: The factorial of 0 is 1.
4. What will `factorial(5)` return?
5. What is the factorial of `6`?

---

## **Quiz Answers for All Practical Projects**

**Quiz 1:**
1. `print()`
2. `print("text")`
3. Quotes (`'` or `"`)
4. False
5. Hello computer world!

**Quiz 2:**
1. `+`
2. Using the `=` operator (e.g., `num1 = 5`)
3. 8
4. False
5. 12

**Quiz 3:**
1. `-`
2. 7
3. True
4. 10
5. 10

**Quiz

4:**
1. `if`
2. Using comparison operators (`>`, `<`, etc.)
3. False
4. Larger
5. False

**Quiz 5:**
1. `math`
2. `math.sqrt()`
3. True
4. 5.0
5. 6.0

**Quiz 6:**
1. `a, b = b, a`
2. `a = 20`, `b = 10`
3. False
4. Swaps the values of `a` and `b`
5. `a = 10`, `b = 5`

**Quiz 7:**
1. 0.621371
2. Using the `*` operator (e.g., `km * 0.621371`)
3. 3.106855
4. True
5. 6.21371 miles

**Quiz 8:**
1. `(Celsius * 9/5) + 32`
2. 32.0
3. True
4. 212°F
5. -40°F

**Quiz 9:**
1. Least Common Multiple
2. By using a loop or a mathematical formula to find the smallest common multiple
3. True
4. 15
5. 24

**Quiz 10:**
1. Highest Common Factor
2. Greatest Common Divisor (GCD)
3. True
4. 4
5. 5

**Quiz 11:**
1. `while condition:`
2. Using `i += 1`
3. False
4. 1 2 3
5. 1, 2, 3, 4, 5, 6, 7, 8, 9, 10

**Quiz 12:**
1. `for element in sequence:`
2. Using a `for` loop (e.g., `for char in string`)
3. True
4. P Y T H O N
5. P, Y, T, H, O, N

**Quiz 13:**
1. `input()`
2. Using a `for` loop (e.g., `for i in range(n)`)
3. True
4. 
    ```python
    *
    **
    ***
    ```
5. 
    ```python
    *
    **
    ***
    ****
    ```

**Quiz 14:**
1. Using `def` (e.g., `def function_name():`)
2. `length * breadth`
3. True
4. (15, 16)
5. 30

**Quiz 15:**
1. `append()`
2. Using `[]`
3. True
4. `[1, 2, 3, 4]`
5. `[10, 20, 5]`

**Quiz 16:**
1. Using curly braces `{}` (e.g., `my_dict = {}`)
2. Dictionary
3. True
4. Alice
5. Using `dict[key] = value`

**Quiz 17:**
1. `n! = n * (n-1) * (n-2) * ... * 1`
2. Using `def` and calling the function within itself
3. True
4. 120
5. 720

---

This completes the quizzes for all the practical projects in **Unit 7**. These questions and answers will help you assess your understanding of the key programming concepts covered in this unit.

---
