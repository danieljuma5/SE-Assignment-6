[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15475081&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a high-level, interpreted programming language known for its readability and simplicity. Some key features include:

- **Easy to Read and Write**: Python's syntax is straightforward and mirrors human language.
- **Interpreted Language**: Python code is executed line-by-line, which makes debugging easier.
- **Dynamically Typed**: Variable types are determined at runtime, making coding faster and more flexible.
- **Large Standard Library**: Python comes with a vast library of modules and packages for various tasks.
- **Community Support**: Python has a large and active community, contributing to numerous third-party libraries and frameworks.

**Use Cases:**

- **Web Development**: Using frameworks like Django and Flask.
- **Data Science and Machine Learning**: Libraries like NumPy, pandas, and scikit-learn.
- **Automation and Scripting**: Automating repetitive tasks.
- **Software Development**: Building desktop and server-side applications.
- **Scientific Computing**: Libraries like SciPy and Matplotlib.



2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   **Windows:**

1. Download Python installer from [python.org](https://www.python.org/).
2. Run the installer and ensure "Add Python to PATH" is checked.
3. Follow the installation prompts.

4. Verify installation: Open Command Prompt and type `python --version`.
5. Create a virtual environment: 
   `
   python -m venv myenv
`

   **MacOS**

 -  Open Terminal.
   Install Homebrew (if not installed):
   ```markdown
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
   - Install Python:
<code>
brew install python
</code>
- Verify installation:
<code>
python3 --version
</code>
- Create a virtual environment:
```
python3 -m venv myenv
```
- Activate the virtual environment:
```
source myenv/bin/activate
```
**Linux**
- Open Terminal.
- Install Python:
```
sudo apt-get update
sudo apt-get install python3
```
- Verify installation:
```
python3 --version
```
- Install venv module:
```
sudo apt-get install python3-venv
```
- Create a virtual environment:
```
python3 -m venv myenv
```
- Activate the virtual environment:
```
source myenv/bin/activate
```
3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   Linux:
```
print("Hello, World!")
```
Explanation:

- **print:** A built-in function to display output to the console.
- **"Hello, World!":** A string literal enclosed in double quotes.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

**Basic Data Types:**

 - **int**: Integer numbers.
- **float**: Floating-point numbers.
 - **str**: Strings (text).
- **bool**: Boolean values (True or False).
- **list**: Ordered collection of items.
- **tuple**: Ordered, immutable collection of items.
- **dict**: Key-value pairs.
 - **set**: Unordered collection of unique items.
 ```
 # Integer
a = 10
print(a, type(a))

# Float
b = 20.5
print(b, type(b))

# String
c = "Hello"
print(c, type(c))

# Boolean
d = True
print(d, type(d))

# List
e = [1, 2, 3]
print(e, type(e))

# Tuple
f = (4, 5, 6)
print(f, type(f))

# Dictionary
g = {"name": "Alice", "age": 25}
print(g, type(g))

# Set
h = {7, 8, 9}
print(h, type(h))
```

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   Conditional Statements:

**Used to execute code based on certain conditions.**

Example:

```
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is 5 or less")
```
**Loops:**

Used to iterate over a sequence of elements.

For Loop Example:

```
for i in range(5):
    print(i)
```

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   Functions are reusable blocks of code that perform a specific task. They help to organize and modularize code, making it more readable and maintainable.

Example:

```
def add(a, b):
    return a + b
```
**Calling the function**
```
result = add(3, 5)
print(result)
```
7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Differences:

- **List:** Ordered collection of items, indexed by position, and allows duplicates.
Dictionary: Unordered collection of key-value pairs, indexed by keys, and does not allow duplicate keys.
Script:
```
# List
numbers = [1, 2, 3, 4, 5]
print(numbers)
numbers.append(6)
print(numbers)

# Dictionary
person = {"name": "Alice", "age": 25}
print(person)
person["age"] = 26
print(person)
```

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   Exception Handling:

- **Exception** handling allows you to handle runtime errors gracefully, without terminating the program abruptly.

Example:

```
try:
    x = 10 / 0
except ZeroDivisionError as e:
    print("Error:", e)
finally:
    print("This block always executes")
```
9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.


- **Module**: A single file containing Python code (functions, classes, variables) that can be imported.
- **Package**: A collection of modules in directories that provide a hierarchical namespace.
Example:

```
import math

result = math.sqrt(16)
print(result)
```
10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    Reading from a File:

```
with open('example.txt', 'r') as file:
    content = file.read()
    print(content)
 ```
Writing to a File:

```
lines = ["First line", "Second line", "Third line"]
with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + "\n")
```
# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


