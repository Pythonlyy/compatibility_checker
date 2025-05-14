# 💘 Operators & Expressions: Compatibility Checker Project

Welcome to **Chapter 2**: Operators & Expressions! This beginner-friendly project teaches you how to use Python's core operators — arithmetic, comparison, logical, and even string operations — by building a playful and interactive **Compatibility ŕChecker**.

---

## 📌 What You'll Learn

* ✅ How to use arithmetic operators: `+`, `-`, `*`, `/`, `**`, `%`
* ✅ Comparison operators: `==`, `!=`, `<`, `>`, `>=`, `<=`
* ✅ Logical operators: `and`, `or`, `not`
* ✅ String operations: concatenation and repetition
* ✅ How to get user input with `input()`

---

## 💡 About the Project

In this project, the user inputs two names. The program then uses a mix of math, logic, and string operations to generate a **fun compatibility score**. The result is based on the length of each name, some playful math, and a few simple checks. It's not scientifically accurate 😉 — but it's a great way to:

* Understand how Python handles basic expressions
* See how data can be manipulated with logic
* Practice writing and testing conditional code
* Build something interactive in just a few lines

This kind of mini app is the perfect step between printing "Hello World" and building full applications.

---

## 🧱 Project Code

```python
# ❤️ Python Compatibility Checker ❤️

# Step 1: Get user input
# Ask the user to type their name and their crush's name
# This lets us work with dynamic input every time the program runs
name1 = input("Enter your name: ")
name2 = input("Enter your crush's name: ")

# Step 2: Combine names and show string math
# Demonstrates string concatenation and repetition
combined = name1 + name2
print("\nYour names combined:", combined)
print("Repeated 3 times:", combined * 3)

# Step 3: Compatibility logic using math and comparison
# We calculate a score based on the length of each name
# The formula uses basic arithmetic and the modulo operator (%) to keep it within 0-99
score = (len(name1) * 3 + len(name2) * 2) % 100
print("\nYour compatibility score is:", score, "%")

# Step 4: Use logical conditions to give a message
# Based on the score, we use conditional statements to print different outcomes
if score > 80:
    print("🔥 You two are a power couple!")
elif score > 50:
    print("😊 You have potential — worth a shot!")
elif score > 30:
    print("🙅️‍♂️ Hmm... could go either way.")
else:
    print("💔 Better as friends, maybe!")

# Step 5: Use comparison and logical operators explicitly
# Just for fun, we explore additional Boolean logic and comparisons
# These print statements evaluate to True or False
print("\nFun fact checks:")
print("Are your names the same length?", len(name1) == len(name2))
print("Is either name longer than 10 characters?", len(name1) > 10 or len(name2) > 10)
print("Is the score over 90 and both names short?", score > 90 and len(name1) < 5 and len(name2) < 5)
```

---

## 🧪 Breakdown of Concepts

| Concept               | Used In                    |
| --------------------- | -------------------------- |
| `+`, `*` on strings   | `combined = name1 + name2` |
| `input()`             | Getting user input         |
| `len()`               | Measuring string length    |
| Arithmetic operations | Calculating score          |
| Comparison operators  | If/elif logic              |
| Logical operators     | Fun fact checks            |

---

## 🧮 How to Run This Project

1. Make sure you have **Python 3** installed.
2. Save the code above in a file called `compatibility_checker.py`
3. Open your terminal and run:

   ```bash
   python compatibility_checker.py
   ```

---

## 🌟 Try These Bonus Challenges:

* Ask for user ages and include them in the score logic
* Add a retry feature to test multiple pairs
* Export results to a text file
* Make a GUI version using `tkinter`
* Create a scoring system that factors in initials or total character count

---

---

🐍 This is part of the **Pythonly beginner series**.
Learn Python one line at a time. Follow [@Pythonly](https://github.com/Pythonlyy) for more.
