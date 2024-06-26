[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15294091&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is a high-level, interpreted programming language known for its readability, simplicity, and versatility. 
Some of its key features include:
Readability and simplicity- python's syntax is clear and easy to read resembling natural language.
Python has an extensive standard library that includes modules and packages for a wide range of tasks eliminating reliance on third-party libraries.
Python supports procedural, object-oriented, and functional programming, giving developers flexibility in how they approach problem-solving and can run on various operating systems without needing modifications.
Python has a large and active community that contributes to a wealth of resources, including tutorials, documentation, and forums, which helps in learning and problem-solving.
Python's web frameworks, such as Django, streamline the development of web applications, libraries like NumPy, and Matplotlib make Python ideal for data manipulation, analysis, and visualization.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

Visit https://www.python.org/ and navigate to downloads where the latest version compatible with windows will be suggested. Click to download. Locate the downloaded folder in your device and run the installer. During installation,  check the box that says "Add Python to PATH" and continue with the default installation settings and wait for the installation to complete. To verify the installation, open command prompt an dexecute the command "python --version". You can also check the pip version by executing "pip --version".
To install a virtual environment, execut the command "pip intall virtualenv". To create a virtual environment,navigate to the project directory and type "python -m virtualenv environmentname". To activate the virtual environment, execute "source environmentname/ Scripts/activate". To deactivate, type "deactivate" and press enter.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   print("Hello, World!")
   Synatx: The print() function is used to output text to the console. The arguments to be printed are enclosed in parenthesis.
   A string is a sequence of characters enclosed in quotes (double or single). The string in this case is "Hello, World!".

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   
   How to create and use the variables is written in square brackets[]
   Integer (int)- represents whole numbers. [age=30] [print("Age:", age)]
   Floating point (float)- represents real numbers that may include decimals. [height=7.9] [print("Height:", height)]
   Boolean (bool)- represents logical values, either True or False. [is_student = True] [print("Is student:", is_student)]
   List- represents ordered collections of items, which can be of different data types. [fruits = ["apple", "banana", "cherry"] ] [print("Fruits:", fruits)]
   Dictionaries- represents collections of key-value pairs. [person = {"name": "Bob", "age": 25}] [print("Person:", person)]

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements and loops in python allow one to control the flow of your program based on certain conditions and to repeat actions. Conditional statements allow one to execute different blocks of code based on certain conditions. Loops allow you to repeat a block of code multiple times.
   
   Example of an if-else statement:
   age = 20
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
   
   Example of a for loop:
   fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python are blocks of reusable code that perform a specific task. Functions are useful because they allow for code reusability, they help break down complex problems into manageable pieces, they make code easier to read and understand and easier to maintain.
   Example:
   def add_two_numbers(a, b): 
   return a + b

   result = add_two_numbers(3, 5)
   print("The sum is:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists maintain the order of items and each item has a specific index while dictionaries do not maintain the order of items and items are stored as key-value pairs.
   
   An example of a list:
   numbers= [1, 2, 3, 4, 5]
   print("Original list: ", numbers)
   numbers.append(6)
   print("After appending 6: ", numbers)
   numbers.remove(3)
   print("After removing 3: ", numbers)
   print("Number at index 2: ",numbers[2])

   An example of a dictionary:
   person= {"name" : "Doe", "age" : "25", "town" : "Nairobi"}
   print("Original dictionary: ", person)
   person["email"]= "doe@gmail.com"
   print("After adding email: ", person)
   del person["town"]
   print("After deleting town: ", person)
   print("Name: ",person["name"])

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python is a mechanism to handle runtime errors, allowing the program to continue execution or terminate gracefully. It helps manage unexpected errors by catching them and providing an appropriate response, rather than letting the program crash.
   Example:
   def divide_numbers(a, b):
    try:
        result = a / b
    except ZeroDivisionError:
        print("Error: Cannot divide by zero.")
        result = None
    else:
        print("Division successful.")
    finally:
        print("Execution completed.")
    return result

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   A module is a single file containing Python definitions and statements which allows you to logically organize your Python code. A package is a way of organizing related modules into a directory hierarchy that is essentially a directory with a special __init__.py file that can contain initialization code for the package. To use a module in your script you need to import it using "import module_name".
   Example:
   import math
   number = 16
   square_root = math.sqrt(number)
   print(f"The square root of {number} is {square_root}")

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file. 

    To read from a file;
    Open the file using 'open()' in read mode, read the content using methods like 'read()' and cloose using methods using 'close()'.
    Example:
    def read_file(file_path):
    try:
        with open(file_path, 'r') as file:
            content = file.read()
            print(content)
    except FileNotFoundError:
        print(f"The file {file_path} does not exist.")
    except IOError:
        print(f"An error occurred while reading the file {file_path}.")

   file_path = 'example.txt'
   read_file(file_path)

   To write to a file;
   Open the file using 'open()' in write/append mode, write the content using methods like 'write()' and cloose using methods using 'close()'.
   Example:
   def write_to_file(file_path, lines):
    try:
        with open(file_path, 'w') as file:
            for line in lines:
                file.write(line + '\n')
        print(f"Content written to {file_path} successfully.")
    except IOError:
        print(f"An error occurred while writing to the file {file_path}.")

   file_path = 'output.txt'
   lines_to_write = [
       "Hello, World!",
      "This is a test file.",
      "It contains multiple lines of text.",
      "Goodbye!"
   ]
   write_to_file(file_path, lines_to_write)

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


