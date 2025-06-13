# This script was created as part of my Intro to Python coursework at Rose State College. It calculates geometric properties of a sphere using user input and Python’s math module.

Project Description: Sphere Calculations
This Python program calculates the diameter, circumference, surface area, and volume of a sphere based on user input for the radius. I chose to write the code in a simple, readable way using built-in functions and the math module to demonstrate a solid understanding of variables, input/output, and basic arithmetic operations.

Why I Coded It This Way:
User Input: I used input() and float() to accept radius values so the program can handle decimals, which are common in real-world measurements.

Math Module: I imported math to access the constant math.pi for more precise calculations.

Clear Variable Names: Each geometric formula is broken down into individual variables (diameter, circumference, etc.) to make the code easy to understand and debug.

Formatted Output: I used f-strings to neatly print the results with descriptive labels, and I rounded the output to 2 decimal places using the round() function for a cleaner, more professional presentation.

Structured & Commented: The code includes a header comment block explaining the assignment prompt so that anyone reading the code—including future employers—can quickly understand the project’s purpose.

This structure mirrors how real-world developers are expected to write code: readable, well-documented, and user-friendly. It also reflects the kinds of tasks covered in early programming or CompTIA certification objectives—connecting math, logic, and Python fundamentals.

Pop Culture Tie-In
Like Iron Man building his suit with precision and calculations, this program turns math into function. In cybersecurity and tech, accuracy and process matter just as much as creativity—and that starts with the basics.

References
Whitman, M. E., & Mattord, H. J. (2018). Management of Information Security (6th ed.). Cengage Learning.

Python Software Foundation. (n.d.). Python Documentation. Retrieved from https://docs.python.org/

GeeksforGeeks. (n.d.). Python math Module. Retrieved from https://www.geeksforgeeks.org/python-math-module/


---

What This Program Does (in plain English):

The program asks the user to **enter the radius of a sphere**, then calculates:

* The **diameter**
* The **circumference**
* The **surface area**
* The **volume**

It uses mathematical formulas to compute those values and then **prints the results** nicely using formatted output.

---

Line-by-Line Breakdown:

1. `import math`

This line pulls in Python’s built-in **math module**, which gives us access to constants and functions like `math.pi` (which represents π ≈ 3.14159). Without this, we’d have to manually type out pi.

---

2. `radius = float(input("Enter the radius of the sphere: "))`

This line:

* Shows a **message** to the user asking for the radius
* Uses `input()` to grab what they type
* Wraps that input in `float()` to **convert** it to a number with decimals (like `5.2` instead of just `5`)

You use `float` instead of `int` because the radius of a sphere isn’t always a whole number.

---

3. The Formulas:

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

4. Why use `round()`?

```python
round(circumference, 2)
```

Python will sometimes spit out **long decimal numbers** like `31.41592653589793`. That’s accurate, but not user-friendly.

`round(value, 2)` makes it easier to read by **rounding to 2 decimal places** (like `31.42`). This is cleaner, especially when showing results to users or on a report.

So you’re balancing:

* Accuracy (from `math.pi`)
* Simplicity (from `round()`)

---

5. f-Strings:

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

Recap:

> I used Python’s `math` module to access pi accurately, and `float()` to accept decimal input for the radius. I used standard formulas for sphere measurements, and applied `round()` to make the results readable and professional. I formatted my print statements using f-strings for clean and modern output. This makes the program user-friendly while still accurate.




