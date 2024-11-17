<!--
ID: PYTHON-BE-001
Tags: [python, beginner, programming, training]
Description: A beginner-level Python exercise focusing on basic programming concepts.
Query: Generate a beginner-level getting started training exercise for python. Display every step of the entire training exercise as a wiki file in a markdown-formatted string that I can copy or download. Make the exercise very positive and detailed. Include all prerequisites and steps. Add a hidden field to the top of the exercise with the following parameters: ID, Tags, Description, Query, Model, Level. Where ID is a unique ID. Where Tags is a list of tags associated with the exercise. Where Description is a short overview of the exercise. Where Query is this query string. Where model is the model and version of the LLM that I'm submitting the query to. Where level is the skill level of this exercise rated as beginner, intermediate, or advanced.
Model: ChatGPT v2
Level: beginner
-->

# Getting Started with Python: A Beginner's Exercise

Welcome to your first Python programming exercise! This guide will walk you through the basics of Python, covering fundamental concepts and giving you hands-on experience. By the end of this exercise, you'll have a solid understanding of Python basics and will have written your first Python program.

## Prerequisites

Before you begin, ensure you have the following:

1. **Python Installed**: Download and install Python from the official website [python.org](https://www.python.org/). Python 3.x is recommended.
2. **Code Editor**: Choose a code editor to write your Python code. Options include:
   - **Visual Studio Code**: [Download here](https://code.visualstudio.com/)
   - **PyCharm**: [Download here](https://www.jetbrains.com/pycharm/download/)
   - **Sublime Text**: [Download here](https://www.sublimetext.com/)
3. **Basic Computer Skills**: Familiarity with basic computer operations and navigation.

## Steps

### 1. **Set Up Your Environment**

1. **Install Python**:
   - Download Python from [python.org](https://www.python.org/downloads/).
   - Follow the installation instructions for your operating system (Windows, macOS, Linux).
   - Ensure the option to add Python to your PATH is checked during installation.

2. **Verify Python Installation**:
   - Open your command line or terminal.
   - Type `python --version` and press Enter. You should see the installed version of Python.
   - Optionally, you can use `python3 --version` if your system differentiates between Python 2 and 3.

### 2. **Write Your First Python Script**

1. **Open Your Code Editor**:
   - Launch the code editor you installed.

2. **Create a New File**:
   - In your editor, create a new file and name it `hello.py`.

3. **Write Code**:
   - In `hello.py`, type the following code:

     ```python
     # This is a simple Python program that prints "Hello, World!"
     print("Hello, World!")
     ```

4. **Save Your File**:
   - Save the file with the `.py` extension.

### 3. **Run Your Python Script**

1. **Open Command Line or Terminal**:
   - Navigate to the directory where you saved `hello.py` using the `cd` command.

2. **Execute Your Script**:
   - Type `python hello.py` and press Enter. If your system uses `python3`, type `python3 hello.py` instead.
   - You should see `Hello, World!` printed to the screen.

### 4. **Explore Basic Python Concepts**

1. **Variables**:
   - Variables are used to store data. For example:

     ```python
     name = "Alice"
     age = 30
     print(name)
     print(age)
     ```

2. **Data Types**:
   - Python supports various data types, including integers, floats, strings, and lists. Try experimenting with these:

     ```python
     number = 10          # Integer
     pi = 3.14            # Float
     greeting = "Hello!" # String
     numbers_list = [1, 2, 3, 4, 5] # List

     print(number, pi, greeting)
     print(numbers_list)
     ```

3. **Functions**:
   - Functions are blocks of code that perform a specific task. Define a function and call it:

     ```python
     def greet(name):
         return f"Hello, {name}!"

     print(greet("Bob"))
     ```

4. **Control Flow**:
   - Use `if` statements to control the flow of your program:

     ```python
     age = 18
     if age >= 18:
         print("You are an adult.")
     else:
         print("You are a minor.")
     ```

### 5. **Practice and Experiment**

- Try modifying the code snippets provided to see how changes affect the output.
- Explore more Python concepts such as loops, error handling, and file operations.

## Conclusion

Congratulations on completing your first Python exercise! You’ve learned the basics of Python programming and written a simple script. Keep practicing and exploring more features of Python to build your programming skills.

Happy coding!

