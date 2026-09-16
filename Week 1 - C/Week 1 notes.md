# Week 1 — C

In Week 1, we moved from Scratch to C, which was my first introduction to programming with a traditional programming language.
This week helped me understand more about what is actually happening between the code I write and the machine executing that code.
Machine Code, Source Code and Compilers
I learned that machine code is the low-level language consisting of instructions represented in binary that the computer’s processor can execute.
The code that I write as a programmer is called source code.
A compiler is a program that translates source code into another form that can eventually be executed by the computer, including machine code.

## The Terminal
I learned about the terminal, which is an interface where I can enter commands and interact with the computer using text.
I also learned about two major ways of interacting with computers:
GUI — Graphical User Interface
CLI — Command Line Interface
The GUI allows us to interact with a computer through graphical elements such as windows, icons and buttons, while the CLI allows us to enter text commands.

## Escape Sequences
I learned that certain characters have special meanings in C.
For example: \n represents a new line.
This is called an escape sequence.
I also learned about other escape sequences, including:
\n - new line
\r - carriage return
\" - double quotation mark
\' - single quotation mark
\\ - backslash

They allow us to represent characters that would otherwise have a special meaning to the compiler.

## Reading Error Messages
I learned how important compiler error messages are when debugging.
For example, if I see:
hello.c:5:29
this tells me that the error is associated with:
hello.c → the file
5 → line 5
29 → character/column 29

## Header Files and Libraries
I learned that C has header files, which commonly end in .h.
For example:
#include <stdio.h>
stdio.h is a header file that provides declarations for standard input/output functionality, including functions such as printf.

I also learned that programmers don’t have to write every piece of functionality themselves. Libraries contain code and functionality that can be reused.
CS50 also provides its own header files and libraries for the course.

## Variables and Data Types
I learned that variables have types.
A variable declaration generally specifies: type variable_name;
For example: int age; or: string name; depending on the type and the CS50 functionality being used.
The type tells the compiler what kind of data the variable is intended to hold.

## printf
I learned that printf is used to print formatted output to the terminal.
For example: printf("Hello, %s\n", answer);
Here: "Hello, %s\n" is the format string. %s is a placeholder for a string. \n moves the cursor to a new line. answer is the value that will replace %s.
The comma separates the format string from the values that are supplied to the placeholders.

I also learned that C statements generally end with a semicolon.
For example: printf("Hello\n");
The semicolon terminates the statement.

## Format Specifiers
I learned about several format specifiers used with printf:
%s - string
%d - integer
%li - long integer
%f - floating-point value
%c - character
These allow printf to know how to interpret the value being inserted into the output.

## Data Types
I learned about several data types in C, including:
bool
char
double
float
int
long
string (provided through CS50’s library)
I also learned some of their typical sizes:
float → 32 bits
double → 64 bits
int → typically 32 bits
long → typically 64 bits on the CS50 environment
I learned that the exact size of some C types can depend on the system, so these shouldn’t always be assumed to be universal.

## Characters
I learned that a single character can be represented using the char data type.
For example: char letter = 'A';
This is different from a string, which can contain multiple characters.
I also learned that when comparing individual characters, we use char values.

## Conditionals
I learned how to use conditionals in C.
The basic structure is:
if (condition)
{
    // code
}
This allows the program to execute certain instructions only when a particular condition is true.

## Operators
I also learned about operators such as:
+ addition
- subtraction
* multiplication
/ division
% remainder/modulus
== equal to
!= not equal to
< less than
> greater than
<= less than or equal to
>= greater than or equal to

## Loops
I learned that loops allow us to repeat code.
The main loop structures in C are:
while
do ... while
for
I also learned about scope.
For example, if a variable is declared inside a loop or another block of code, it generally cannot be accessed outside that block.

## Functions
I learned how to create functions in C.
The keyword: void can indicate that a function returns no value. It can also be used as the parameter list to indicate that a function takes no arguments.

For example:
void hello(void)
{
    // code
}
In this example:
The first void means the function returns no value.
The second void means the function takes no arguments.

## Function Prototypes
I learned that the compiler processes C source code from top to bottom.
Because of this, if I define a function after main, the compiler needs to know about that function before main tries to use it.
This is where a function prototype comes in.
For example:
void hello(void);

int main(void)
{
    hello();
}

void hello(void)
{
    printf("Hello\n");
}
The prototype:
void hello(void); acts as a declaration that tells the compiler that this function exists and will be defined later.
I found the idea of a function prototype interesting because it is essentially a declaration or “promise” to the compiler about the function.

## Comments
I learned that: // is used to write a single-line comment in C.
For example: // This is a comment
Comments are ignored by the compiler and are mainly used to explain code to humans.

## Linux / Terminal Commands
I learned several basic terminal commands:
cd -change directory
ls - list files/directories
mkdir - create a directory
rm - remove a file
rmdir - remove an empty directory
mv - move or rename a file
cp- copy a file

One important distinction I learned is that cd does not create a directory. It changes the current working directory.

## Correctness, Design and Style
I learned about three important aspects of programming:
### Correctness
Does the program actually do what it is supposed to do?
### Design
Is the program structured efficiently and logically?
### Style
Is the code readable and understandable?
I learned that a program can be correct while still having poor design or poor style.
This was an important distinction because writing code isn’t only about making something that works. It is also about making code that other people can understand and maintain.

## const
In the mario.c example, I learned about: 'const' which is used to declare a variable whose value should not be changed after it has been initialized.
For example: const int MAX = 8;
This helps prevent accidental modification of values that are supposed to remain constant.

## Integer Overflow
In the calculator.c example, I learned about integer overflow.
Computers have a finite amount of memory available for representing numbers. If a number becomes larger than the maximum value that can be represented by a particular integer type, the result can overflow.
The Boeing 737 example was particularly interesting to me because it demonstrated how a relatively small numerical error can eventually have significant real-world consequences.
This helped me understand that integer overflow isn’t just a theoretical programming problem—it can have practical consequences when software deals with real-world systems.

## Type Casting
I learned about type casting, which allows a value to be converted from one data type to another.
For example: (float) x can convert an integer value stored in x into a floating-point value.
This is particularly useful when performing calculations where I need to preserve decimal values.

## Floating-Point Precision
I learned about floating-point imprecision.
Computers cannot represent every possible decimal number exactly using binary floating-point representation.
Because of this, calculations involving floating-point numbers can sometimes produce results that are slightly different from what we mathematically expect.
For example, a computer might not represent a number such as 0.1 exactly.
This is something I want to understand more deeply as I continue learning programming.

## Controlling Decimal Places
I also learned that printf allows me to control the number of decimal places displayed for a floating-point value.
For example: printf("%.2f\n", value); prints the value to 2 decimal places.
Similarly: printf("%.5f\n", value); prints it to 5 decimal places.
The number after the decimal point specifies the number of digits to display after the decimal point.

### Overall Reflection

Week 1 was a major step up from Scratch because I started seeing what programming actually looks like in a traditional programming language.
I learned about:
Machine code
Source code
Compilers
The terminal
GUIs and CLIs
Escape sequences
Error messages
Header files
Libraries
Variables
Data types
Format specifiers
printf
Conditionals
Operators
Loops
Scope
Functions
Function prototypes
Comments
Linux commands
Correctness, design and style
Constants
Integer overflow
Type casting
Floating-point imprecision

The biggest thing I took away from this week is that programming is not just about memorizing syntax. There is a lot happening underneath the code, from how information is represented in binary to how the compiler interprets what I write.

## Next step: Continue with the Week 1 C problem set.