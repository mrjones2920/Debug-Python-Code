# Debug Python Code

<h1>Introduction</h1>
One of the biggest challenges faced by analysts is ensuring that automated processes run smoothly. Debugging is an important practice that security analysts incorporate in their work to identify errors in code and resolve them so that the code achieves the desired outcome.

Through a series of tasks in this lab, you'll develop and apply your debugging skills in Python.

<h1>Scenario</h1>
In your work as a security analyst, you need to apply debugging strategies to ensure your code works properly.

Throughout this lab, you'll work with code that is similar to what you've written before, but now it has some errors that need to be fixed. You'll need to read code cells, run them, identify the errors, and adjust the code to resolve the errors.

<h1>Task 1</h1>
The following code cell contains a syntax error. In this task, you'll run the code, identify why the error is occuring, and modify the code to resolve it. (To ensure that it has been resolved, run the code again to check if it now functions properly.)

![image](https://github.com/user-attachments/assets/8d8b3297-2518-4c1b-aa99-2344712628fc)

<h1>Question 1</h1>
What happens when you run the code before modifying it? How can you fix this?

When the code is run before it's modified, the output shows SyntaxError: invalid syntax, which indicates that there is a syntax error. The syntax error is caused by the missing : at the end of the for loop header. To fix this, you can add : at that position.

<h1>Task 2</h1>
In the following code cell, you're provided a list of usernames. There is an issue with the syntax. In this task, you'll run the cell, observe what happens, and modify the code to fix the issue.

![image](https://github.com/user-attachments/assets/1116f27f-8a64-450f-90e4-c7272ca1b2c4)

<h1>Question 2</h1>
What happens when you run the code before modifying it? How can you fix it?

When the code is run before it's modified, the output shows SyntaxError: invalid syntax. The issue occurred when assigning a value to usernames_list. The fourth username is missing a closing quotation mark, and there is a missing comma between the fourth and fifth usernames. Each username in the list should be a string, and commas should be used to separate one username from the next. To fix the syntax error, you can add a closing quotation mark to properly specify the fourth username as a string and then add a comma between the fourth and fifth usernames to separate them. So instead of "zdutchma "esmith",, it should say "zdutchma", "esmith",.

<h1>Task 3</h1>
In the following code cell, there is a syntax error. Your task is to run the cell, identify what is causing the error, and fix it.

![image](https://github.com/user-attachments/assets/040393ca-4f6b-46dd-a9fe-4f4ccd9e38d0)

<h1>Question 3</h1>
What happens when you run the code before modifying it? What is causing the syntax error? How can you fix it?

When the code is run before it's modified, the output shows SyntaxError: unexpected EOF while parsing. This is caused by the missing closing paranthesis at the end of the print() statement. To fix this, you can add ) at the end of the line.

<h1>Task 4</h1>
In the following code cell, you're provided a usernames_list, a username, and code that determines whether the username is approved. There are two syntax errors and one exception. Your task is to find them and fix the code. A helpful debugging strategy is to focus on one error at a time and run the code after fixing each one.

![image](https://github.com/user-attachments/assets/46a0aa6f-66c1-4459-b1af-cd1c7849b351)

<h1>Question 4</h1>
What happens when you run the code before modifying it? What is causing the errors? How can you fix it?

When the code is run before it's modified, the output shows SyntaxError: invalid syntax, as that's the first error that Python encounters in this code. There are three issues in the code:

In the if condition, the = assignment operator is used instead of the == comparison operator, causing a syntax error. To fix this, you can replace = with ==.
Inside the if statement, indentation is missing, causing a syntax error. To fix this, you can add appropriate indentation before the print() statement.
The variable usernames_list is misspelled in the for loop condition. It's spelled as username_list there, causing an exception. To fix this, you can add the missing s in the appropriate spot.
<h1>Task 5</h1>
In this task, you'll examine the following code and identify the type of error that occurs. Then, you'll adjust the code to fix the error.

![image](https://github.com/user-attachments/assets/d2089d17-c822-419b-9a86-fcb7882ddbbd)

<h1>Question 5</h1>
What happens when you run the code before modifying it? What type of error is this? How can you fix it?

When the code is run before it's modified, the output shows IndexError: list index out of range, which means that there is an index error, and it's caused by an invalid index value that is being used with a list. Note that an index error is a type of exception in Python. Also, recall that indexing in Python starts at 0 and the usernames_list has a length of 5. So 4 is the index value corresponds to the final element in usernames_list. 5 is not a valid index in usernames_list. You can fix the error by replacing 5 with 4.

<h1>Task 6</h1>
In this task, you'll examine the following code. The code imports a text file into Python, reads its contents, and stores the contents as a list in a variable named ip_addresses. It then removes elements from ip_addresses if they are in remove_list. There are two errors in the code: first a syntax error and then an exception related to a string method. Your goal is to find these errors and fix them.

![image](https://github.com/user-attachments/assets/756d4419-920a-4eb0-aae1-0caef2538be0)

<h1>Question 6</h1>
What happens when you run the code before modifying it? What is causing the errors? How can you fix them?

When the code is run before it's modified, the output shows SyntaxError: invalid syntax, as that's the first error that Python encounters in this code. There are two errors in the code:

There is a syntax error because the header of the with statement is missing a : at the end. To fix this, you can add : there.
There is an exception related to the string method .split(). To call this method, you must write the name of the variable that contains the string you want to use, followed by a ., and then the name of the method. So to fix, you can replace split.ip_addresses() with ip_addresses.split().

<h1>Task 7</h1>
In this final task, there are three operating systems: OS 1, OS 2, and OS 3. Each operating system needs a security patch by a specific date. The patch date for OS 1 is "March 1st", the patch date for OS 2 is "April 1st", and the patch date for OS 3 is "May 1st".

The following code stores one of these operating systems in a variable named system. Then, it uses conditionals to output the patch date for this operating system.

However, this code has logic errors. Your goal is to assign the system variable to different values, run the code to examine the output, identify the error, and fix it.

![image](https://github.com/user-attachments/assets/da6e3ccf-ea8f-4213-b32e-b292f187c4e5)

<h1>Question 7</h1>
What happens when you run the code before modifying it? What is causing the logic errors? How can you fix them?

When the code is run before it's modified, the system variable is assigned to "OS 2", but the output is Patch date: March 1st. This is not the correct patch date for OS 2.

When assigning system to "OS 1", the output is Patch date: May 1st. This is not the correct patch date for OS 1.

These logic errors are due to the incorrect index values in the first and second print() statements in the code. Note that indexing in Python starts at 0 and patch_schedule is in order of operating system from OS 1 to OS 3. To fix the logic errors, you can use patch_schedule[0] to get the correct patch date for OS 1 and patch_schedule[1] to get the correct patch date for OS 2.

<h1>Conclusion</h1>
What are your key takeaways from this lab?

- Debugging is an essential practice that analysts use to identify errors in code and fix them to ensure that the code runs smoothly.
- Python executes code from top to bottom and stops once it encounters an error. So if there are multiple errors in a code cell, the outputted error message will typically show the first error.
- In Python, common types of errors include syntax errors, logic errors, and exceptions.
- Syntax errors often involve punctuation such as a missing : at the end of a with statement header and a missing , between elements in a list.
- Logic errors could involve incorrect indices when accessing elements from a list.
- Exceptions could involve misspelled variable names or incorrectly called string methods.
- A key strategy for debugging is running code and examining if it produces the intended results. If the output isn't correct, or if it displays an the error message, use this to identify which line(s) of the code could be causing the issue. After fixing the code, it's important to run it again to ensure that everything works as expected.
