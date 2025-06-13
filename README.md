# This script was created as part of my Intro to Python coursework at Rose State College. It calculates geometric properties of a sphere using user input and Python’s math module.

# 🧮 Sphere Calculations in Python

## 📘 Homework Prompt

**Assignment**:  
Write a Python program that takes the radius of a sphere (a floating-point number) as input and then outputs the sphere’s:

- Diameter
- Circumference
- Surface Area
- Volume

Use formulas for sphere geometry and round the output if desired.

---

## 🛠️ What This Program Does

This program asks the user for the radius of a sphere and calculates key geometric values:

- **Diameter** = 2 × radius  
- **Circumference** = 2 × π × radius  
- **Surface Area** = 4 × π × radius²  
- **Volume** = (4/3) × π × radius³  

It then prints each value, neatly formatted and rounded to two decimal places.

---

## 🎯 Why I Coded It This Way

I designed this program with clarity, simplicity, and readability in mind:

- **User Input**: The radius is entered as a floating-point number to allow decimal precision.
- **Modular Design**: Each formula is stored in its own variable so the logic is clear and beginner-friendly.
- **Python’s `math` Module**: I used `math.pi` to get an accurate and consistent value of π.
- **Formatted Output**: I used Python f-strings and the `round()` function to display results professionally and clearly.
- **Well-Documented**: The code includes comments and a top block with the assignment prompt so others (including future employers) can easily understand the context.

---

## 💡 What I Learned

- How to accept and process floating-point user input in Python.
- How to use the `math` module for precise scientific constants.
- How to structure output using f-strings for clean, human-readable display.
- The importance of documentation and clean code—especially when saving projects to GitHub for future reference.

---

## 📁 File

- `sphere_calculations.py`: The main script file for this project.

---

## 📌 Example Output

```text
Enter the radius of the sphere: 4.5

Diameter: 9.0
Circumference: 28.27
Surface Area: 254.47
Volume: 381.7
````

---

## 🧠 Pop Culture Tie-In

Like Iron Man building his suit with precision and calculations, this program turns math into function. In cybersecurity and tech, accuracy and process matter just as much as creativity—and that starts with the basics.

---

## 📚 References

* Whitman, M. E., & Mattord, H. J. (2018). *Management of Information Security* (6th ed.). Cengage Learning.
* Python Software Foundation. (n.d.). *Python Documentation*. Retrieved from [https://docs.python.org/](https://docs.python.org/)
* GeeksforGeeks. (n.d.). *Python math Module*. Retrieved from [https://www.geeksforgeeks.org/python-math-module/](https://www.geeksforgeeks.org/python-math-module/)

---
## 🧠 What This Program Does (in plain English):

```text

The program asks the user to **enter the radius of a sphere**, then calculates:

* The **diameter**
* The **circumference**
* The **surface area**
* The **volume**

It uses mathematical formulas to compute those values and then **prints the results** nicely using formatted output.

```

---

## 🧩 Line-by-Line Breakdown:

### 1. `import math`

This line pulls in Python’s built-in **math module**, which gives us access to constants and functions like `math.pi` (which represents π ≈ 3.14159). Without this, we’d have to manually type out pi.

---

### 2. `radius = float(input("Enter the radius of the sphere: "))`

This line:

* Shows a **message** to the user asking for the radius
* Uses `input()` to grab what they type
* Wraps that input in `float()` to **convert** it to a number with decimals (like `5.2` instead of just `5`)

You use `float` instead of `int` because the radius of a sphere isn’t always a whole number.

---

### 3. The Formulas:

```python
diameter = 2 * radius
circumference = 2 * math.pi * radius
surface_area = 4 * math.pi * radius ** 2
volume = (4 / 3) * math.pi * radius ** 3
```

These are **standard math formulas** for spheres:

| Quantity      | Formula             |
| ------------- | ------------------- |
| Diameter      | 2 × radius          |
| Circumference | 2 × π × radius      |
| Surface Area  | 4 × π × radius²     |
| Volume        | (4/3) × π × radius³ |

The `**` symbol is the exponent operator in Python.
So `radius ** 2` means *radius squared*, and `radius ** 3` means *radius cubed*.

---

### 4. Why use `round()`?

```python
round(circumference, 2)
```

Python will sometimes spit out **long decimal numbers** like `31.41592653589793`. That’s accurate, but not user-friendly.

`round(value, 2)` makes it easier to read by **rounding to 2 decimal places** (like `31.42`). This is cleaner, especially when showing results to users or on a report.

So you’re balancing:

* Accuracy (from `math.pi`)
* Simplicity (from `round()`)

---

### 5. f-Strings:

```python
print(f"Circumference: {round(circumference, 2)}")
```

The `f` in `f""` stands for **formatted string**. It lets you:

* Write text
* Embed Python expressions using `{}` directly inside the string

So you get readable output like:

```python
f"My favorite number is {math.pi}"
```

Without f-strings, you’d have to write something messier like:

```python
print("Circumference: " + str(round(circumference, 2)))
```

---

## 🗣️ Recap:

> I used Python’s `math` module to access pi accurately, and `float()` to accept decimal input for the radius. I used standard formulas for sphere measurements, and applied `round()` to make the results readable and professional. I formatted my print statements using f-strings for clean and modern output. This makes the program user-friendly while still accurate.

