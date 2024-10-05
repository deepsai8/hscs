# **Unit 5c: Tuples and Dictionary**

---

## **Introduction**

In Python, **tuples** and **dictionaries** are important data structures that help organize and manage collections of data. Tuples are immutable sequences of values, while dictionaries are collections of key-value pairs that allow you to associate values with specific keys. In this unit, you’ll learn how to work with tuples and dictionaries, including how to create, access, and manipulate them.

---

## **5c.1 Tuples**

A **tuple** is an ordered, immutable collection of items in Python. Once created, the elements in a tuple cannot be changed, which makes tuples useful for data that should remain constant throughout the program.

### **Creating and Initializing Tuples**
You can create a tuple by placing values inside parentheses `()`, separated by commas.

**Example**:
```python
my_tuple = (1, 2, 3)
fruit_tuple = ("apple", "banana", "cherry")
```

### **Accessing Elements in a Tuple**
Just like with lists, you can access elements in a tuple using **indexing**. Indexing starts at 0.

**Example**:
```python
my_tuple = (1, 2, 3)
print(my_tuple[0])  # Outputs: 1
```

### **Operations on Tuples**
Although tuples are immutable, you can perform various operations:

1. **Concatenation**: Combine two or more tuples using the `+` operator.

    **Example**:  
    ```python  
    tuple1 = (1, 2)  
    tuple2 = (3, 4)  
    combined_tuple = tuple1 + tuple2  # Outputs: (1, 2, 3, 4)  
    ```  

2. **Repetition**: Repeat a tuple multiple times using the `*` operator.

    **Example**:  
    ```python  
    repeat_tuple = (1, 2) * 3  # Outputs: (1, 2, 1, 2, 1, 2)  
    ```  

3. **Slicing**: Extract a subset of the tuple using a range of indices.

    **Example**:  
    ```python  
    my_tuple = (1, 2, 3, 4, 5)  
    print(my_tuple[1:4])  # Outputs: (2, 3, 4)  
    ```  

4. **Length**: Find the number of elements in a tuple using the `len()` function.

    **Example**:  
    ```python  
    my_tuple = (1, 2, 3)  
    print(len(my_tuple))  # Outputs: 3  
    ```  

5. **Membership**: Check if an item is present in a tuple using the `in` keyword.

    **Example**:  
    ```python  
    fruit_tuple = ("apple", "banana", "cherry")  
    print("banana" in fruit_tuple)  # Outputs: True  
    ```  

---

## **5c.2 Dictionary**

A **dictionary** in Python is an unordered, mutable collection of items. Each item is stored as a **key-value pair**, where the key acts as an identifier and the value is the data associated with the key. Dictionaries are commonly used when you need to associate one piece of data with another, such as a name with a phone number.

### **Creating and Initializing Dictionaries**
Dictionaries are created using curly braces `{}`, with each key-value pair separated by a colon `:`. Keys must be unique and immutable (e.g., strings, numbers), while values can be any data type.

**Example**:
```python
my_dict = {"name": "Alice", "age": 25, "city": "New York"}
```

### **Accessing Elements in a Dictionary**
You can access the value associated with a key by using the key in square brackets.

**Example**:
```python
my_dict = {"name": "Alice", "age": 25, "city": "New York"}
print(my_dict["name"])  # Outputs: Alice
```

### **Dictionary Operations**

Dictionaries allow various operations:

1. **Adding or Modifying Elements**: You can add new key-value pairs or modify existing ones.

    **Example**:  
    ```python  
    my_dict["age"] = 26  # Modifies the value of "age"  
    my_dict["email"] = "alice@example.com"  # Adds a new key-value pair  
    ```  

2. **Removing Elements**: You can remove a key-value pair using the `del` keyword or `pop()` method.

    **Example**:  
    ```python  
    del my_dict["city"]  # Removes the key "city"  
    age = my_dict.pop("age")  # Removes the key "age" and returns its value  
    ```  

3. **Traversing a Dictionary**: You can loop through a dictionary’s keys, values, or both using a `for` loop.

    **Example**:  
    ```python  
    for key, value in my_dict.items():  
      print(key, value)  
    ```  

4. **Checking for a Key**: You can check if a key exists in the dictionary using the `in` keyword.

    **Example**:  
    ```python  
    if "name" in my_dict:  
      print("Name found")  
    ```  

5. **Getting the Length**: Use `len()` to find the number of key-value pairs in the dictionary.

    **Example**:  
    ```python  
    print(len(my_dict))  # Outputs: 3  
    ```  

---

## **Important Terminology**

- **Tuple**: An ordered, immutable collection of elements.
- **Dictionary**: An unordered, mutable collection of key-value pairs.
- **Key-Value Pair**: A pair where a key identifies a specific value in a dictionary.
- **Mutability**: The ability to change the contents of a data structure (e.g., dictionaries are mutable, while tuples are immutable).

---

## **Quiz**

1. What is the difference between a list and a tuple?  
    a) Tuples are mutable, and lists are immutable  
    b) Lists are immutable, and tuples are mutable  
    c) Tuples are immutable, and lists are mutable  
    d) Tuples and lists are both immutable  

2. How do you access the second element of a tuple `my_tuple = (10, 20, 30)`?  
    a) `my_tuple[2]`  
    b) `my_tuple[1]`  
    c) `my_tuple[0]`  
    d) `my_tuple[-1]`  

3. True or False: Tuples can be modified after creation.  

4. Which of the following is used to create a dictionary?  
    a) Square brackets `[]`  
    b) Parentheses `()`  
    c) Curly braces `{}`  
    d) Double quotes `""`  

5. How do you access the value associated with the key `"name"` in the dictionary `my_dict = {"name": "Alice", "age": 25}`?  
    a) `my_dict.get("Alice")`  
    b) `my_dict["Alice"]`  
    c) `my_dict.get("name")`  
    d) `my_dict["name"]`  

6. True or False: Dictionary keys must be unique.  

7. Which of the following is an example of a key-value pair in a dictionary?  
    a) `"name": "Alice"`  
    b) `"age": 25`  
    c) `25: "Alice"`  
    d) All of the above  

8. What does the following code do?  
    ```python  
    del my_dict["age"]  
    ```  
    a) Removes the value `"age"` from the dictionary  
    b) Removes the key `"age"` and its associated value from the dictionary  
    c) Clears all elements from the dictionary  
    d) Modifies the value of `"age"`  

9. What method is used to remove and return a value from a dictionary by key?  
    a) `del()`  
    b) `pop()`  
    c) `remove()`  
    d) `clear()`  

10. True or False: A dictionary’s values must be unique.  

---

## **Answers**

1. c) Tuples are immutable, and lists are mutable
2. b) `my_tuple[1]`
3. False
4. c) Curly braces `{}`
5. d) `my_dict["name"]`
6. True
7. d) All of the above
8. b) Removes the key `"age"` and its associated value from the dictionary
9. b) `pop()`
10. False

---

This unit has introduced you to tuples and dictionaries, two essential data structures in Python. You’ve learned how to create, access, and manipulate these structures, giving you the ability to manage complex collections of data efficiently in your programs.

---
