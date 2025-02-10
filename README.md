# INET 3101 Lab 1
## Created by Wendy Vang

- Program Description: User is provided with a menu in which they can enter various descriptions about parts through a command-line menu. They may also be able to view various statistics about the database and make modifications to the database as well. Once the user is finished working with the command-line menu, they may exit the menu and their modifications will be saved upon exiting the menu.


- Menu Definition & Usage: Through the menu, the user can print all records currently in the database, add a record, delete a record, print the number of records in the database, print the database's size, print the number of changes, or exit.

- Files Required: Standard C Library Header (stdio.h) in order to use functions such as scanf and printf.

# Functions

## printRecords()
- **Input Type:** None  
- **Output Type:** None  
- **Description:**  
  For now, it simply prints a statement stating that the function has been entered by the user.  

## addRecord()
- **Input Type:** None  
- **Output Type:** None  
- **Description:**  
  Prompts the user to run through a few variables regarding part descriptions and then prints out what the user has inputted for each description of the part.  

## deleteRecord()
- **Input Type:** None  
- **Output Type:** None  
- **Description:**  
  For now, it simply prints a statement stating that the function has been entered by the user.  

## numberOfRecords()
- **Input Type:** None  
- **Output Type:** None  
- **Description:**  
  For now, it simply prints a statement stating that the function has been entered by the user.  

## databaseSize()
- **Input Type:** None  
- **Output Type:** None  
- **Description:**  
  For now, it simply prints a statement stating that the function has been entered by the user.  

## printChanges()
- **Input Type:**  
  - `int selection` → User determines through an integer whether they want to see how many times the database has been modified or if they'd like to increment the amount of modifications by 1.  
  - `int *modifications` → Pointer to the variable modifications so that changes are reflected outside of the function.  

- **Output Type:** None  

- **Description:**  
  Prompts the user to make a selection between seeing how many modifications have been made to the database or incrementing the modification counter by 1. Regardless of selection, a print statement displaying the amount of modifications made to the database will be displayed.  

## main()
- **Input Type:**  
  - `int argc` → Keeps track of how many arguments are being inputted into the program, such as whether or not a database name has been provided when attempting to run the code.  
  - `char *argv[]` → Pointer to a character array, which keeps track of what is being inputted into the code when it is being executed through the terminal.  

- **Output Type:**  
  - `int` → Mainly to indicate termination of the program once the user is done.  

- **Description:**  
  Prompts the user to go through the command-line menu, where they can summon specific commands to modify or view the database. Each command will call the appropriate method to carry out its function. Once the user is done, they may exit the program by inputting `7`.  
