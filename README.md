#!/bin/bash   # <---This is NOT a comment. It is called "Sha-Bang"; it tells the operating system where the bash interpreter is located, the path to the interpreter.

# Working with Variables
# Variables created when assigned value = Dynamic typing
# Variable names can contain numbers and characters.
# Variable names are case sensitive.
# There should not be any space around '=' sign when assigning a value
PRICE_PER_APPLE=5
MyFirstLetters=ABC
greetings='Hello		world!'

# $Variable_Name or ${Variable_Name} can be used to reference a variable. The ${} is used to avoid ambiguity.
echo "${PRICE_PER_APPLE}" # or echo $PRICE_PER_APPLE
echo "${MyFirstLetters}" # or echo $MyFirstLetters
# ... and so on.

# Take look at the variable greetings, now try the following
echo $greetings
# observe that the number of spaces between words "Hello" and "world" has reduced to one.
# To preserve the whitespaces in the output use double quotes
echo "$greetings"

# Aliases can be create using back-ticks or $(), as below
all_visible_and_hidden_files_folders=`la -la`
echo $all_visible_and_hidden_files_folders # or "$all_visible_and_hidden_files_folders"

today_date=$(date +%Y-%m-%d)
echo `date` # (or just date) It will print the date in a pretty descriptive format, now execute the following and see the difference in the output.
echo $today_date

# See the code in birthday.sh script
