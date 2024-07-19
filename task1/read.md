Task List Application Documentation

Overview

The Task List Application is a simple console-based application that allows users to manage a list of tasks. The application provides options to add tasks, remove tasks, list tasks, and quit the application.

Design Choices

Java as the programming language: Java was chosen as the programming language for its platform independence, object-oriented design, and large community support.
Console-based interface: A console-based interface was chosen for its simplicity and ease of implementation.
ArrayList for task storage: An ArrayList was chosen for storing tasks due to its dynamic size and ease of manipulation.
Scanner for user input: A Scanner was chosen for reading user input from the console.
Implementation

The implementation consists of two classes: TaskListApp and TaskList.

TaskListApp Class

The TaskListApp class is the main class of the application and contains the main method. It is responsible for:

Creating a TaskList object to store tasks.
Creating a Scanner object to read user input from the console.
Displaying the menu to the user and reading the user's choice.
Processing the user's choice and performing the corresponding action.
TaskList Class

The TaskList class is responsible for managing the list of tasks. It provides methods to:

Add a task to the list.
Remove a task from the list.
List all tasks in the list.
Check if the list is empty.
Check if a task number is valid.
Changes Made

To change the data type of the task name from int to String, the following changes were made:

In the TaskList class, the addTask method was modified to accept a String parameter instead of an int parameter.
In the TaskListApp class, the getTaskName method was modified to return a String instead of an int.
In the TaskListApp class, the case 1 block was modified to call the getTaskName method and pass the returned String to the addTask method.
Challenges Faced

Handling invalid user input: One of the challenges faced was handling invalid user input, such as non-integer values when expecting an integer input. This was resolved by using try-catch blocks to catch InputMismatchException and NumberFormatException.
Validating task numbers: Another challenge was validating task numbers to ensure they are within the range of available tasks. This was resolved by adding a isValidTaskNumber method in the TaskList class.
