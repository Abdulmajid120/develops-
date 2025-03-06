#BASH SCRIPTING ASSIGHNMNET 

##Basic Arithmetic - Write a script that takes two numbers as input
from the user and performs basic arithmetic operations (addition,
subtraction, multiplication, and division) and then displays all the
answers of those operations in the terminal.

1.	#!/bin.bash 
Read -p “enter first number “ num1
Read -p “enter second number” num2 
Sum=$((num1+num2))
Echo “the sum of num1 and num2 is “
If [[ $sum -eq 24 ]]; then
Echo “congratulations you’re a genius”.
Else
Echo “try again”
Fi
###File Operations - Write a script that creates a directory, navigates
into it, creates a file inside it, writes some text to the file, and then
displays the contents of the file.

2.	#! /bin.bash
mkdir England
cd England
touch London 
echo "good morning London" > London  
cat London
####Conditional Statements - Write a script that checks if a file exists and
prints a message indicating whether it exists or not. If it exists, the
script should also check if the file is readable, writable, or executable.

3.	#!/bin/bash

if [ -f "London" ]; then
echo "There you are!"
else
    echo "Your lost"
fi

 #####Backup Script - Create a script that copies all .txt files from a
specified directory to a backup directory. If the backup directory
doesn’t exist, the script should create it first.

4.	#!/bin/bash

if [ -d "England" ]; then
    mkdir -p Backup  
    cp England/*.txt Backup/
    echo "Files copied successfully!"
else
    echo "England directory does not exist. Creating it now..."
    mkdir -p England
    echo "England directory created no .txt files to copy yet."
fi
