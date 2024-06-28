[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15320759&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

  Python is a high-level programming language used in writing simple and readable code.
  key features that make python popular is simple to read and debug, It has extensive libraries and frameworks as well as large community for support.
  Python is effective in Web development, machine learning, data analysis, game development

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   To install python, download and install from www.python.org
   verify installation by running script in terminal 

   bash
   python --version

   Install virtual environment using pip installer: 

   bash
   pip install virtualenv

   Navigate to project directory:

bash

cd my_project

Create a virtual environment:
bash

virtualenv venv
Activate the Virtual Environment:

bash

./venv/Scripts/activate


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   print("Hello, World!")

   Print: prints output text to the console or display.
   String "Hello, World!" : Is the sequence of character in quoteation marks (single ''/double "") to be displayed.
   Parentheses (): The parentheses are used to pass arguments to the function


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Integer (int): Whole number either positive or negative without decimal. e.g 10 , -2.

   Floating point numbers (float): Numbers with decimal points. e.g 3.14, -2.0.

   Strings (str): A sequence of characters enclosed in quotes.
   e.g "James", 'james'.

   Booleans (bool): Represents either True or False. e.g True, False.

   Lists (list): Ordered, mutable collection of items, which can be of mixed data types. e.g [1, 2, 3], ['yam', 'banana', 'vanilla'].

   Tuples (tuple): Ordered, immutable collection of items
   e.g (1, 2, 3), ('apple', 'banana', 'cherry').

   Dictionaries (dict): Unordered collection of items identified by key and value pairs.

   e.g {'name': 'steve', 'age': 65}, {'fruit': 'apple', 'color': 'green}.

   Sets (set): collection of unique sets items.
   e.g {1, 2, 3}, {'apple', 'banana', 'cherry'}.

   Script that demonstrates how to create and use variables of different data types:

   age = 65;
   print(f"Age: {age} ({type(age)}))

    Dictionary
person = {"name": "steve", "age": 65}
print(f"Person: {person} (Type: {type(person)})")


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements are used to perform different actions based on different conditions. E.g if,else and if else.
   syntax : if (condition):
   e.g if age >= 18:
   print("Welcome, pick your entery voucher")
   else:
   print("Entry Not Allowed")

   The (for) used to execute a block of code repeatedly as long as a certain condition is satisfied.
   e.g 
   person = ["steve", "Nathan" , "Neville"]
   for person in persons:
   print(person)
   //Output
   steve
   Nathan
   Neville


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions are blocks of code designed to perform a specific which can be reused in the program.

   Importance:
   1. They make the code more manageable and easier to debug.
   2. Reuse code across different parts of a program or even different programs
   e.g
   def add_num(7,9):
      return(7+9)

   result = add_num(7+9)
   print(result) //16



7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists (list): Ordered, mutable collection of items, which can be of mixed data types.
    e.g [1, 2, 3], ['yam', 'banana', 'vanilla'].
    Lists are initialised by square brackets ([]) with there values separated by comma (,)

    Dictionaries (dict): Are Unordered collection of items identified by key and value pairs.
    They are initialised by caly braces.
# e.g
   person = {
    "name": "steve",
    "age": 37,
    "city": "Nairobi"
   }

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling in Python is a way to manage errors that may occur during the execution of a program.

   try : The code that might raise an exception is placed inside the try block.

   except: The code that runs if an exception occurs in the try block is placed inside the except block.

   finally: The code inside the finally block always runs, regardless of whether an exception occurred or not. 

   # e.g 
   def (a,b):
      try:
         result = a / b
      except ZeroDivisionError as e:
         print("Cannot divide by zero")
      except TypeError as e:
             print("Error: Both arguments must be numbers.")
        result = None
    finally:
        print("Execution of the try-except-finally block is complete.")
    return result

# e.g
print("Result of division:", divide_numbers(10, 2))
print("Result of division:", divide_numbers(10, 0))
print("Result of division:", divide_numbers(10, "a"))

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.


 Modules and Packages define functions, classes, and variables, which can be reused in other Python scripts
 import math

# Using functions from the math module
print("Square root of 16:", math.sqrt(16)) 
# Output: 4.0
print("Value of pi:", math.pi)              
# Output: 3.141592653589793

print("Cosine of 0:", math.cos(0))

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

# Reading a file 
    def read_file(Plp_modules):
    try:
       
        with open(Plp_modules, 'r') as file:
            
            for line in file:
                print(line.strip())  
    except FileNotFoundError:
        print(f"Error: The file '{Plp_modules}' does not exist.")
    except IOError:
        print(f"Error: Failed to read the file '{Plp_modules}'.")

# Example usage:
Plp_modules = 'Assignment.txt'  
read_file(Plp_modules)

# Writing a list of strings to a file


def write_to_file(Plp_modules, lines):
    try:
 # Open the file       
        with open(Plp_modules, 'w') as file:
 # Add a newline after each line           
            for line in lines:
                file.write(line + '\n')  
        print(f"Successfully wrote {len(lines)} lines to '{Plp_modules}'.")
    except IOError:
        print(f"Error: Failed to write to the file '{Plp_modules}'.")

# Example usage:
Plp_modules = 'Assignment.txt' 
Text_to_add  = [
    "I have completed my PLP software Engineering module assignment 6."]
write_to_file(Plp_modules, Text_to_add)


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


