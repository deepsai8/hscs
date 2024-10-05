# **Unit 2: Encoding Schemes and Number Systems**

---

## **Introduction:**

In this unit, we’ll explore how computers represent data using encoding schemes and different number systems. While humans typically think in terms of decimal numbers (0-9), computers communicate and store information using other systems, like binary (0 and 1). You’ll also learn how to convert between different number systems, which is a fundamental skill in computer science. Let’s break down these concepts and make them fun and easy to understand!

---

## **2.1 Encoding Schemes:**

Computers work with numbers, not letters or symbols. To help computers understand our alphabets, numbers, and even emojis, encoding schemes are used. An **encoding scheme** converts characters (like letters and punctuation) into numeric codes so that computers can store and process them.

### **ASCII (American Standard Code for Information Interchange):**

ASCII was developed as one of the earliest encoding schemes to standardize how computers represent text and symbols. It uses **7 bits** to encode 128 different characters, including:
- **Uppercase and lowercase letters** (A-Z, a-z)
- **Numbers** (0-9)
- **Special symbols** (such as @, &, #, and punctuation marks)
- **Control characters** (like Enter, Tab, and Backspace)

**Example:**
- The ASCII code for the letter **A** is **65**.
- The ASCII code for the symbol **@** is **64**.

However, ASCII is limited. Since it uses only 7 bits, it can only represent **128 characters**, which is not enough for languages other than English or for newer symbols like emojis.

---

### **UNICODE:**

To address the limitations of ASCII, **UNICODE** was developed. It can represent over **143,000 characters** from a variety of languages and symbol sets, making it a universal encoding scheme. UNICODE uses **16 bits** or more to represent characters, allowing it to handle different writing systems such as:
- **Latin** (for English and other languages)
- **Cyrillic** (for Russian and related languages)
- **Chinese characters**
- **Emojis** (Yes, even your favorite emojis like 😃 have unique UNICODE numbers!)

UNICODE has become the global standard for encoding characters in digital text, ensuring that all languages and symbols can be represented consistently across different platforms.

**Example:**
The smiley emoji **😃** has a UNICODE value of **U+1F603**.

**Why is UNICODE important?**
With the world connected through the internet, we need a system that represents characters from every language. Whether you're writing in English, Russian, or Japanese, or sending an emoji, UNICODE makes sure the computer understands what you’re saying.

---

## **2.2 Number Systems:**

In computing, different **number systems** are used to represent and process data. While we humans typically use the **decimal system** (Base 10), computers use the **binary system** (Base 2) because they can only process two states: **on (1)** and **off (0)**.

---

### **Decimal Number System (Base 10):**

The decimal system is the one we use every day. It’s called **Base 10** because it uses ten digits: 0, 1, 2, 3, 4, 5, 6, 7, 8, and 9. We can represent any number using these digits by placing them in positions that are powers of 10.

**Example:**
- The number **125** in decimal is represented as:
  \[
  1 \times 10^2 + 2 \times 10^1 + 5 \times 10^0 = 100 + 20 + 5 = 125
  \]

This is how we naturally count, but it’s not suitable for computers.

---

### **Binary Number System (Base 2):**

Computers use the **binary system**, which is based on **two digits**: 0 and 1. This system is called **Base 2** because it only has two possible values. Every binary digit (bit) represents a power of 2, just as every decimal digit represents a power of 10.

**Example:**
- The binary number **101** means:
  \[
  1 \times 2^2 + 0 \times 2^1 + 1 \times 2^0 = 4 + 0 + 1 = 5
  \]

While binary numbers may seem long, they are crucial for computers because they map directly to the on/off states of electronic circuits.

**Fun Fact:**
Think of binary like a light switch: **1** means "on" and **0** means "off." Your computer is flipping millions of these "switches" every second to perform tasks!

---

### **Octal Number System (Base 8):**

The **octal system** uses eight digits: 0, 1, 2, 3, 4, 5, 6, and 7, and is based on **Base 8**. It was commonly used in early computers because it’s easier to convert between binary and octal than between binary and decimal.

**Example:**
- The octal number **17** means:
  \[
  1 \times 8^1 + 7 \times 8^0 = 8 + 7 = 15 \text{ in decimal}
  \]

---

### **Hexadecimal Number System (Base 16):**

The **hexadecimal system** uses **16 symbols**: the digits 0-9 and the letters A-F, where:
- **A = 10**
- **B = 11**
- **C = 12**
- **D = 13**
- **E = 14**
- **F = 15**

This system is very useful in computing because it allows large binary numbers to be represented more compactly.

**Example:**
- The hexadecimal number **1A** means:
  \[
  1 \times 16^1 + A \times 16^0 = 16 + 10 = 26 \text{ in decimal}
  \]

**Why Hexadecimal?**
Hexadecimal is often used in programming and computing because it’s easier to work with than long strings of binary numbers. For example, the binary number **11111111** can be written more compactly as **FF** in hexadecimal.

---

## **2.3 Converting Between Number Systems:**

Understanding how to convert between different number systems is a core skill in computer science. Let’s look at some conversion techniques:

---

### **Decimal to Binary:**

To convert a decimal number to binary:
1. **Divide** the decimal number by 2.
2. **Write down the remainder** (0 or 1).
3. **Continue dividing** the result by 2, writing down the remainders, until the quotient is 0.
4. **The binary number** is the sequence of remainders read in reverse order.

**Example:**
Convert **13** to binary.
13 ÷ 2 = 6 remainder **1**
6 ÷ 2 = 3 remainder **0**
3 ÷ 2 = 1 remainder **1**
1 ÷ 2 = 0 remainder **1**
So, **13** in decimal is **1101** in binary.

---

### **Binary to Decimal:**

To convert a binary number to decimal:
1. **Multiply each bit** by \(2^n\), where **n** is the position of the bit, starting from 0 on the right.
2. **Add the results**.

**Example:**
Convert **1101** to decimal.
\(1 \times 2^3 + 1 \times 2^2 + 0 \times 2^1 + 1 \times 2^0 = 8 + 4 + 0 + 1 = 13\).

---

### **Decimal to Hexadecimal:**

To convert a decimal number to hexadecimal:
1. **Divide the decimal number** by 16.
2. **Write down the remainder** (0-9, A-F).
3. **Continue dividing** the result by 16 until the quotient is 0.
4. **The hexadecimal number** is the sequence of remainders read in reverse order.

**Example:**
Convert **255** to hexadecimal.
255 ÷ 16 = 15 remainder **15 (F)**
15 ÷ 16 = 0 remainder **15 (F)**
So, **255** in decimal is **FF** in hexadecimal.

---

### **Hexadecimal to Decimal:**

To convert a hexadecimal number into decimal:
1. **Multiply each digit** by \(16^n\), where **n** is the position of the digit, starting from 0 on the right.
2. **Add the results**.

**Example:**
Convert **1A** to decimal.
\(1 \times 16^1 + A \times 16^0 = 16 + 10 = 26\).

---

## **Important Terminology:**

- **Encoding:** The process of converting characters into a numerical format for computers to understand.
- **ASCII:** An encoding scheme that represents English characters and symbols using 7 bits.
- **UNICODE:** A more extensive encoding scheme that represents characters from multiple languages and symbols, including emojis.
- **Decimal:** The number system humans commonly use (Base 10).
- **Binary:** The number system computers use, consisting of only 0s and 1s (Base 2).
- **Octal:** A number system that uses eight digits (0-7) (Base 8).
- **Hexadecimal:** A number system that uses 16 symbols (0-9 and A-F) (Base 16).

---

## **Quiz:**

1. What is the purpose of an encoding scheme?  
    a) To convert text into images  
    b) To represent characters as numbers  
    c) To calculate binary numbers  
    d) To manage computer memory  

2. What does ASCII stand for?  
    a) American Standard Code for Information Interconnection  
    b) American Standard Code for Information Interchange  
    c) Advanced Symbol Code for International Information  
    d) Application System Code for Internet  

3. Which of the following can be represented using UNICODE but not ASCII?  
    a) The letter "A"  
    b) The number "9"  
    c) The emoji 😃  
    d) The symbol "#"  

4. True or False: The binary system uses only 0 and 1.  

5. What is **1101** in decimal?  
    a) 11  
    b) 12  
    c) 13  
    d) 14  

6. How many symbols does the hexadecimal system use?  
    a) 2  
    b) 8  
    c) 10  
    d) 16  

7. Convert the decimal number **255** into hexadecimal.  
    a) FF  
    b) FE  
    c) F1  
    d) 1F  

8. True or False: UNICODE can represent characters from all writing systems, including emojis.  

9. What is the octal representation of the decimal number **17**?  
    a) 21  
    b) 20  
    c) 17  
    d) 10  

10. Convert the hexadecimal number **A5** to decimal.  
     a) 105  
     b) 165  
     c) 175  
     d) 195  

---

## **Answers:**

1. b) To represent characters as numbers
2. b) American Standard Code for Information Interchange
3. c) The emoji 😃
4. True
5. c) 13
6. d) 16
7. a) FF
8. True
9. d) 10
10. b) 165

---
