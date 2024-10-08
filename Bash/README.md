# Bash Examples

## First Bash Program

Code:

```bash
echo "Hello world!"
```

Output:

```text
Hello world!
```

## Echo commands

Code:

```bash
echo "Printing text with newline"
echo -n "Printing text without newline" # '-n' to print any text without a new line
echo -e "\nRemoving \t backslash \t characters" # '-e' command to remove backslash characters
```

Output:

```text
Printing text with newline
Printing text without newline
Removing         backslash       characters
```

## Use of comment

Code:

```bash
# Add two values
sum=$((30 + 20))
 
# Thereafter print the result
echo $sum
```

Output:

```text
50
```

## Multiline comment

Code:

```bash
: '
The script written below is used to calculate the square of 2
 '
area=$((2 * 2))
echo $area
```

Output:

```text
4
```

## While Loop

Code:

```bash
valid=true
count=1

while [ $valid ]
do
    echo $count

    if [ $count -eq 5 ] # -eq -> equal
    then 
        break
    fi
    ((count++))
done
```

Output:

```text
1
2
3
4
5
```

## For Loop

Code:

```bash
for (( counter=10; counter>0; counter-- ))
do
    echo -n "$counter " # '-n' to print any text without a new line
done

printf "\n"
```

Output:

```text
10 9 8 7 6 5 4 3 2 1
```

## Get User Input

Code:

```bash
echo -n "Enter your name: " # '-n' to print any text without a new line
read name
echo "Welcome $name to Linux!"
```

Output:

```text
Enter your name: Luis
Welcome Luis to Linux!
```

## If statement

Code:

```bash
echo -n "Enter an integer number: " # '-n' to print any text without a new line
read s

if (( $s%2 == 0 ))
then
    echo "It is divisible by 2!"
else
    echo "It is not divisible by 2!"
fi
```

Output:

```text
Enter an integer number: 5
It is not divisible by 2!
```

## Use of if statement together with AND logic

Code:

```bash
echo -n "Input username: " # '-n' to print any text without a new line
read username
echo -n "Input password: " # '-n' to print any text without a new line
read password

if [[ ( $username == "main" && $password == "users" ) ]] 
then
    echo "Valid user!"
else
    echo "Invalid user!"
fi
```

Output:

```text
Input username: main
Input password: users
Valid user!
```

## Use if statement with OR logic

Code:

```bash
echo -n "Enter any number: " # '-n' to print any text without a new line
read s

if [[ ( $s -eq 10 || $s -eq 40 ) ]]
then
    echo "Well played!"
else
    echo "Sorry, you failed!"
fi
```

Output:

```text
Enter any number: 5
Sorry, you failed!
```

## Use of else if statement

Code:

```bash
echo -n "Enter your lucky number: " # '-n' to print any text without a new line
read n

if [ $n -eq 50 ];
then
    echo "You won the 1st bravo!!!!"
elif [ $n -eq 100 ];
then
    echo "You won the 2nd congrats!!!!"
elif [ $n -eq 500 ];
then
    echo "You won the 3rd congrats!!!!"
else
    echo "Sorry, you have to keep trying pal!"
fi
```

Output:

```text
Enter your lucky number: 5
Sorry, you have to keep trying pal!
```

## Case statement

Code:

```bash
echo -n "Enter your lucky number: " # '-n' to print any text without a new line
read s

case $s in
    50)
        echo echo "You won the 1st bravo!!!!" ;;
    100)
        echo "You won the 2nd congrats!!!!" ;;
    500)
        echo "You won the 3rd congrats" ;;
    *)
        echo "Sorry, you have to keep trying pal!" ;;
esac
```

Output:

```text
Enter your lucky number: 5
Sorry, you have to keep trying pal!
```

## Obtaining arguments from Command Line

Code:

```bash
# Variables $1 and $3 are used to cypher through the first and third command-line arguments, respectively
echo "Total arguments: $#"
echo "1st Argument = $1"
echo "3rd argument = $3"
```

Output:

```text
Total arguments: 3
1st Argument = a
3rd argument = c
```

## Obtain arguments from command-line with names

Code:

```bash
# The cut command slices a line and extracts the text.
# -f option is useful for fixed-length lines.
# Cut uses tab as a default field delimiter but can also work with other delimiter by using -d option. 
for arg in "$@"
do
    index=$(echo $arg | cut -f1 -d=)
    val=$(echo $arg | cut -f2 -d=)
    case $index in
        A) 
            a=$val;;
        B) 
            b=$val;;
        *)
    esac
done

result=$(($a + $b))
echo "A + B = $result"
```

Output:

```text
A + B = 3
```

## Integrated string variables

Code:

```bash
stringA="Linux"
stringB="Mint"
echo "$stringA $stringB"

stringC=$stringA" "$stringB
stringC+=" is the best distro!"
echo $stringC
```

Output:

```text
Linux Mint
Linux Mint is the best distro!
```

## How to obtain a substring of string

Code:

```bash
Str="Linux Mint is the best Distro!"
subStr=${Str:6:4}
echo $subStr
```

Output:

```text
Mint
```

## Addition of two numbers

Code:

```bash
echo -n "Input first number: "
read a

echo -n "Input second number: "
read b

sum=$(($a + $b))
echo "Result = $sum"
```

Output:

```text
Input first number: 3
Input second number: 5
Result = 8
```

## Function creation

Code:

```bash
function x()
{
    echo 'I love Linux!'
}

x
```

Output:

```text
I love Linux!
```

## Functionality creation with parameters

Code:

```bash
Rectangle_Area() {
    area=$(($1 * $2))
    echo "Area is: $area"
}

Rectangle_Area 10 20
```

Output:

```text
Area is: 200
```

## Passing a return a value from a function

Code:

```bash
function greeting() {
    str="Good morning, $fname!"
    echo $str
}

echo -n "Input your fname: "
read fname

val=$(greeting)
echo "Return value of the function is: $val"
```

Output:

```text
Input your fname: Luis
Return value of the function is: Good morning, Luis!
```

## Make Directory

Code:

```bash
echo -n "Input a new directory name: "
read newdir
mkdir $newdir
rm -r $newdir # Remove directory
```

Output:

```text
Input a new directory name: test
```

## Creation of a directory by checking its existence

Code:

```bash
echo -n "New directory name input: "
read ndir

if [ -d "$ndir" ]
then
    echo "The Directory given exists!"
else
    mkdir $ndir
    echo "Directory created!"
    rm -r $ndir # Remove directory
fi
```

Output:

```text
New directory name input: test
Directory created!
```

## Reading a file

Code:

```bash
file='./data/languages.txt'

while read line 
do
    echo $line
done < $file
```

Output:

```text
kotlin
java
php
```

## File Deleting

Code:

```bash
echo -n "Insert a filename to delete: "
read filename
rm -i $filename # -i prompt before every removal
```

Output:

```text
Insert a filename to delete: Example_24.sh
rm: remove regular file 'Example_24.sh'? n
```

## Append or adding to file

Code:

```bash
echo "Before adding the file:"
cat ./data/languages.txt

cp ./data/languages.txt ./data/languages_1.txt
echo -e "\nStudying angular" >> ./data/languages_1.txt # >> Appends to a file or creates the file if it doesn't exist.

echo -e "\n\nAfter adding the file: "
cat ./data/languages_1.txt
rm ./data/languages_1.txt
```

Output:

```text
Before adding the file:
kotlin
java
php
python

After adding the file: 
kotlin
java
php
python
Studying angular
```

## Test File existence

Code:

```bash
filename=$1

if [ -f "$filename" ]; then
    echo "File exists!"
else
    echo "File does not exist!"
fi
```

Output:

```text
File exists!
```

## Send Email

Code:

```bash
Recipient="linux@example.com"
Subject="inquiries"
Message="Need anything from linux?"

# <<< Passes the word on the right to the standard input of the command on the left.
mail -s $Subject $Recipient <<< $Message # '-s' option is used in the `mail` command to define the subject of the email.
```

Output:

```text

```

## Parse Current Date

Code:

```bash
Year=`date +%Y`
Month=`date +%m`
Day=`date +%d`
Hour=`date +%H`
Minute=`date +%M`
Second=`date +%S`

echo `date`
echo "Current date is: $Day-$Month-$Year"
echo "Current time is: $Hour:$Minute:$Second"
```

Output:

```text
Mon Jan 8 00:24:33 CST 2024
Current date is: 08-01-2024
Current time is: 00:24:33
```

## The Wait command

Code:

```bash
# Linux OS has a built-in command feature that awaits to complete any running process by using a peculiar id to finish that 
# particular assigned task. Therefore, when there is no job id, the wait command will wait for all secondary cycles to complete 
# before returning exiting. 

# If a command is terminated by the control operator &, the shell executes the command in the background in a subshell. 
# The shell does not wait for the command to finish, and the return status is 0.
echo "Waiting command" & 
process_id=$!
wait $process_id # Wait for process to change state
echo "Exited with status $?"
```

Output:

```text
Waiting command
Exited with status 0
```

## The Sleep Command

Code:

```bash
echo "Please be patient for 5 seconds..."
sleep 5 # Time in seconds
echo "Completed!"
```

Output:

```text
Please be patient for 5 seconds...
Completed!
```

## The AND Operator

Code:

```bash
echo -n "Input a number less than 20: "
read num

if [[ ( $num -lt 20 ) && ( $num%2 -eq 0 ) ]] # -lt->less than, -eq->equal
then
    echo "It is an even number!"
else
    echo "It is an odd number!"
fi
```

Output:

```text
Input a number less than 20: 15
It is an odd number!
```

## The OR Operator

Code:

```bash
echo -n "Enter any number: "
read n

if [[ ( $n -eq 5 || $n -eq 30 ) ]]
then
    echo "You won!"
else
    echo "You lost!"
fi
```

Output:

```text
Enter any number: 15
You lost!
```

## The switch construct

Code:

```bash
echo -n "Input a number: "
read number

case $number in
    50)
        echo "Fifty!!" ;;
    100)
        echo "Double fifty!!" ;;
    *)
        echo "Neither 50 nor 100!" ;;
esac
```

Output:

```text
Input a number: 15
Neither 50 nor 100!
```

## Concatenating strings

Code:

```bash
string1="Linux"
string2="Mint"
string=$string1" "$string2

echo "$string is a great distro!"
```

Output:

```text
Linux Mint is a great distro!
```

## Slicing strings

Code:

```bash
Str="Study smart commands with linux!"
subStr=${Str:0:20}
echo $subStr
```

Output:

```text
Study smart commands
```