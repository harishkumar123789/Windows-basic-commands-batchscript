# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "my-folder"
<img width="367" height="170" alt="image" src="https://github.com/user-attachments/assets/33ddfbe5-327a-4e72-a79d-c51bf170e938" />


## COMMAND AND OUTPUT

Remove the directory "my-folder"
<img width="340" height="147" alt="image" src="https://github.com/user-attachments/assets/995521d6-af08-4b6c-9d39-ef60388d5cf5" />


## COMMAND AND OUTPUT
Create the file Rose.txt
<img width="457" height="57" alt="image" src="https://github.com/user-attachments/assets/2cd5b46d-3ba7-4af3-abba-02b43bede0aa" />

## COMMAND AND OUTPUT
Create the file hello.txt using echo and redirection
<img width="642" height="63" alt="image" src="https://github.com/user-attachments/assets/abe7837a-b640-49a2-ba51-717f62385d44" />


## COMMAND AND OUTPUT

Copy the file hello.txt into the file hello1.txt
<img width="461" height="51" alt="image" src="https://github.com/user-attachments/assets/9a5e88b4-14b2-421b-887a-960c3258dc08" />


## COMMAND AND OUTPUT

Remove the file hello1.txt
<img width="512" height="47" alt="image" src="https://github.com/user-attachments/assets/7e3c33b1-975e-466f-bbd5-0477df6820e5" />


## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".

## OUTPUT
<img width="811" height="205" alt="image" src="https://github.com/user-attachments/assets/bc124d2a-e1b4-4091-9712-20940c53386d" />



Create a batch file  on the desktop that checks whether a user-input number is odd or not. The script should:
Prompt the user to enter a number.
Calculate the remainder when the number is divided by 2.
Display whether the number is odd or not.
Ask the user if they want to check another number.
Repeat the process if the user enters Y, and exit with a thank-you message if the user enters N.
Handle invalid inputs for the continuation prompt (Y/N) gracefully.


## Program
```
@echo off
:menu
echo 1. Say Hello
echo 2. Create a File
echo 3. Exit
set /p choice=Choose an option: 
if "%choice%"=="1" goto hello
if "%choice%"=="2" goto createfile
if "%choice%"=="3" goto end

:hello
echo Hello, World!
goto menu

:createfile
echo Creating a file...
echo This is a new file > newfile.txt
goto menu
:end
echo Goodbye!
pause
```




Use the IF EXIST conditional statement.
Make sure the script works for files located in the same directory as the batch file.
Use pause to keep the command window open after displaying the message.
Expected Output (if the file exists):

<img width="787" height="158" alt="image" src="https://github.com/user-attachments/assets/e61814ad-a60e-4eca-8370-7eb8dcc7ab25" />

## OUTPUT


Write a batch script that displays a simple menu with three options:
Say Hello – Displays the message Hello, World!
Create a File – Creates a file named newfile.txt with the content This is a new file
Exit – Exits the script with a goodbye message
The script should repeatedly display the menu until the user chooses to exit. Use goto statements to handle menu navigation.
<img width="810" height="175" alt="image" src="https://github.com/user-attachments/assets/f4f98826-709b-4341-85b2-46616b27bd5d" />




# RESULT:
The commands/batch files are executed successfully.

