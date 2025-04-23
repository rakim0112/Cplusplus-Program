# Cplusplus-Program Corner Grocer Item Tracking Program
Overview
The Corner Grocer Item Tracking Program is a C++ application designed to track the frequency of items purchased at a grocery store throughout the day. By analyzing text records generated throughout the day, the program helps the store optimize the layout of their produce section based on the purchasing patterns of customers. The program offers four main features:

Search for Item Frequency: Users can input an item and the program will return how often it was purchased.

List All Items and Frequencies: A list of all items with their purchase frequencies is displayed.

Display Histogram: A visual representation (using asterisks) of each item's frequency in a histogram format.

Backup Data: The program creates a backup file (frequency.dat) to store the frequency data of all items purchased.

Problem Solved
The program addresses the need for efficient inventory management in a grocery store. By tracking item purchases, the store can identify which products are bought more frequently and optimize the placement of high-demand items for customer convenience. Additionally, the program offers a backup of the accumulated data, ensuring that no critical information is lost.

Features
Menu Option 1: Prompt a user to input an item and returns its purchase frequency.

Menu Option 2: Displays a list of all items along with their respective purchase frequencies.

Menu Option 3: Displays a histogram where each item is followed by a number of asterisks representing its frequency.

Menu Option 4: Exits the program.

Data Backup: A backup file (frequency.dat) is generated, containing the frequency data of all items.

How to Use
Run the Program: Start the application in a C++ environment (Visual Studio or other IDE).

Input File: Ensure that the input text file (CS210_Project_Three_Input_File.txt) containing the list of items is placed in the same directory as the program. The file should contain the list of produce items purchased, one per line.

Use the Menu: Choose from the menu options to interact with the program:

Option 1: Search for a specific item and get its frequency.

Option 2: Print a list of all items and their frequencies.

Option 3: View a histogram of item frequencies.

Option 4: Exit the program.

The program will generate a frequency.dat file with the item frequencies for backup purposes.

Code Structure
Class Definitions:
ItemTracker: The class that manages item frequency counts using a map. This class contains methods to:

Read from the input file.

Count the frequency of each item.

Display the frequency list.

Display the histogram.

Write the backup data to a file.

Key Functions:
countItemFrequencies(): Reads the input file and counts the frequency of each item.

displayFrequencyList(): Prints out each item and its corresponding frequency.

displayHistogram(): Prints out a histogram for the frequency of each item using asterisks.

backupData(): Writes the frequency data to a backup file.

Reflection
1. Summarize the project and what problem it was solving.
The project aims to track and display the frequency of items purchased at the Corner Grocer. By using this data, the store can optimize the produce layout based on purchasing patterns. The program reads the input file, processes the data, and displays the results in a readable format (list or histogram).

2. What did you do particularly well?
I was able to implement a user-friendly interface with a well-structured menu system. The program correctly handles the input and efficiently stores and displays item frequencies using a map. Additionally, the backup data functionality ensures that the program maintains a record of the results for future use.

3. Where could you enhance your code? How would these improvements make your code more efficient, secure, and so on?
Input validation could be added to ensure that the input file is formatted correctly. For example, I could check for missing or extra values and handle errors gracefully. Additionally, the histogram display could be improved to handle larger datasets more efficiently.

4. Which pieces of the code did you find most challenging to write, and how did you overcome this? What tools or resources are you adding to your support network?
The most challenging part was the file I/O operations, as I needed to ensure that the program could read the input file and write the output correctly without data loss. I overcame this challenge by referring to C++ documentation and tutorials on file handling. I also consulted Stack Overflow and participated in C++ developer forums to get feedback.

5. What skills from this project will be particularly transferable to other projects or coursework?
This project helped me improve my skills in file manipulation, map usage for efficient data storage, and user interface design. These skills will be valuable in future coursework that involves data processing, file handling, and user input validation.

6. How did you make this program maintainable, readable, and adaptable?
I used clear naming conventions for variables and functions, added in-line comments to explain key sections of the code, and broke the program into manageable functions. This structure ensures the program can be easily updated or extended, such as adding more output formats or changing the input file format.

Files Included
item_tracker.cpp: The main source code for the program.

item_tracker.h: Header file for the ItemTracker class.

CS210_Project_Three_Input_File.txt: Sample input file containing the list of produce items purchased.

frequency.dat: Backup data file containing item frequencies.

