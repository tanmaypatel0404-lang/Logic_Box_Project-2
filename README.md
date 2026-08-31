# 🐍 Pattern Generator & Number Analyser

<p align="center">
  <b>A simple Python console application that generates star patterns and analyses numbers.</b>
</p>

<p align="center">
  ⭐ Patterns &nbsp; | &nbsp; 🔢 Number Analysis &nbsp; | &nbsp; 🔄 Loops &nbsp; | &nbsp; 🧠 Python Basics
</p>

---

## 📖 About The Project

**Pattern Generator & Number Analyser** is a beginner-friendly **Python console project** created to practise fundamental programming concepts.

The program provides a simple menu-driven interface where the user can choose between generating a star pattern, analysing a range of numbers, or exiting the program.

### 🎯 The program can:

- ⭐ Generate a right-angled star pattern
- 🔢 Check whether numbers are **Even or Odd**
- ➕ Calculate the sum of numbers in a given range
- ⚠️ Handle invalid inputs such as incorrect ranges
- 🚪 Exit the program safely

---

## 🖥️ Program Menu

When the program starts, the following menu is displayed:

```text
Welcome to the Pattern Generator and Number Analyser

Select an option:
1. Generate a Pattern
2. Analyse a range of Numbers
3. Exit

Enter your choice:
```

---

# ⭐ 1. Pattern Generator

The Pattern Generator asks the user for the number of rows and then creates a right-angled triangle using `*`.

### 💡 Example

**Input:**

```text
Enter your choice: 1

Enter the number of rows for the pattern: 5
```

**Output:**

```text
Pattern
*
**
***
****
*****
```

### 🔧 Logic Used

The pattern is generated using **nested `for` loops**:

```python
for i in range(1, rows + 1):
    for j in range(i):
        print("*", end="")
    print()
```

---

# 🔢 2. Number Analyser

The Number Analyser takes a **starting number** and an **ending number** from the user.

For every number in the range, the program checks whether it is:

- 🟢 **Even**
- 🔵 **Odd**

It also calculates the **total sum** of all numbers in the range.

### 💡 Example

**Input:**

```text
Enter your choice: 2

Enter the start of the range: 1
Enter the end of the range: 5
```

**Output:**

```text
Number 1 is Odd
Number 2 is Even
Number 3 is Odd
Number 4 is Even
Number 5 is Odd

Sum of all numbers from 1 to 5 is: 15
```

### 🔧 Logic Used

The program uses the **modulus operator `%`** to determine whether a number is even or odd:

```python
if i % 2 == 0:
    print("Number", i, "is Even")
else:
    print("Number", i, "is Odd")
```

The sum is calculated using:

```python
total = total + i
```

---

# 🚪 3. Exit

Selecting option `3` exits the program.

```text
Enter your choice: 3

Exiting the program. Goodbye!
```

---

## 🧠 Python Concepts Used

This project helped practise several important Python concepts:

| Concept | Used For |
|---|---|
| 🖨️ `print()` | Displaying output |
| 📥 `input()` | Taking user input |
| 🔢 `int()` | Converting input into integers |
| 🔀 `if / elif / else` | Decision making |
| 🔄 `while` loop | Repeating the menu |
| 🔁 `for` loop | Processing numbers and patterns |
| 🔂 Nested loops | Creating the star pattern |
| ➗ `%` operator | Checking Even/Odd |
| ⛔ `break` | Exiting the program |
| ⏭️ `continue` | Returning to the menu |
| 📏 `range()` | Generating sequences of numbers |

---

## ⚠️ Input Validation

The program also checks for some invalid inputs.

### Invalid Number of Rows

```text
Enter the number of rows for the pattern: 0

Invalid number of rows
```

### Invalid Range

The ending number must be greater than the starting number.

```text
Enter the start of the range: 10
Enter the end of the range: 5

Invalid range
```

### Invalid Menu Choice

```text
Enter your choice: 7

Invalid choice
```

---

## 🔄 How The Program Works

```text
             ┌─────────────────────┐
             │   Start Program 🐍  │
             └──────────┬──────────┘
                        ↓
             ┌─────────────────────┐
             │    Display Menu     │
             └──────────┬──────────┘
                        ↓
              ┌──────────────────┐
              │  Select an option│
              └────────┬─────────┘
                       ↓
       ┌───────────────┼───────────────┐
       ↓               ↓               ↓
   Option 1        Option 2        Option 3
       ↓               ↓               ↓
   Generate       Analyse Range      Exit
   Pattern        Even/Odd + Sum      🚪
       ↓               ↓
       └───────────────┘
               ↓
          Back to Menu
```

---

## 📂 Project Structure

```text
Pattern-Generator-and-Number-Analyser/
│
├── 🐍 main.py
│
└── 📖 README.md
```

> 💡 Replace `main.py` with the actual name of your Python file if it is different.

---

## ⚙️ Requirements

You only need:

- 🐍 **Python 3.x**
- 💻 Any Python IDE or terminal

Check whether Python is installed:

```bash
python --version
```

---

## 🚀 How To Run

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_LINK
```

### 2. Open the project folder

```bash
cd Pattern-Generator-and-Number-Analyser
```

### 3. Run the Python program

```bash
python main.py
```

---

## 🎓 Learning Objective

The main objective of this project is to strengthen the understanding of **Python fundamentals** through a small, practical application.

### Skills practised:

```text
User Input
    ↓
Conditional Statements
    ↓
Loops
    ↓
Nested Loops
    ↓
Arithmetic Operations
    ↓
Input Validation
    ↓
Problem Solving
```

---

## 🚀 Future Improvements

This project can be expanded with more features in the future:

- [ ] 🔺 Add different pattern styles
- [ ] 🔢 Add Prime Number analysis
- [ ] 🏆 Find the largest number in a range
- [ ] 📉 Find the smallest number in a range
- [ ] 📊 Calculate the average
- [ ] ✖️ Generate multiplication tables
- [ ] 🛡️ Handle non-numeric inputs
- [ ] 🎨 Improve the console interface
- [ ] 📋 Add more number-analysis options

---

## 📸 Project Demo

You can add a screenshot of your program here to make your GitHub repository more attractive.

For example:

<img width="457" height="387" alt="Screenshot 2026-08-31 184652" src="https://github.com/user-attachments/assets/0f8601b8-0ffd-4a0b-8da8-bb571e45d39a" />
<img width="505" height="272" alt="Screenshot 2026-08-31 184639" src="https://github.com/user-attachments/assets/c3f4ec63-3562-425d-8b1f-d64590a8f6b8" />

## ▶️ Video Demo



Uploading Proj-2(Logic_box).mp4…





## 👨‍💻 Author

### **Tanmay Patel**

🐍 Python Beginner  
💻 Learning Programming  
🚀 Building Projects & Improving Skills

---

<p align="center">
  ⭐ <b>If you like this project, consider giving it a star!</b> ⭐
</p>

<p align="center">
  Made with 🐍 Python
</p>
