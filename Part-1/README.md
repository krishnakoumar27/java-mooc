## Part 1

Welcome to learning programming! The first part of the course focuses
 on taking the plunge with programming and getting familiar with all the
 required tools.

In this part:

1. Getting started with programming

2. Printing

3. Reading input

4. Variables

5. Calculating with numbers

6. Conditional statements and conditional operation

7. Programming in our society

### Getting started with programming

#### 1. Learning Objectives

- Become familiar with submitting program and learning about Netbeans, etc, 

------------------------------------------------- SKIPPED ------------------------------------------------------

Key terms: 

| term                       | explanation                                                                                                           |
|:--------------------------:| --------------------------------------------------------------------------------------------------------------------- |
| // Write your program here | line comment                                                                                                          |
| Programming                | Designing and implementing software                                                                                   |
| source code                | It is the code we write, consists of statements and expressions, read line from top to bottom and from left to right. |

#### 2. Printing

##### Learning Objectives

- Learn to write a program that prints text.

- Become familiar with executing programs.

- Know what the term "parameter" means.

To print some text:
`System.out.println("Hello world");`

- The information to be printed by the print command, i.e. its **parameters** are passed to it by placing them inside the parentheses () that follow the command.
- commands are seperated by semicolons.

##### Comments

1. Single-line comment - //
2. Multi-line comment - /* */

#### 3. Reading input

##### Learning Objectives

- Learn to write a program that reads text written by a user.
- Know what a "string" refers to in programming.
- Know how to join (i.e., "concatenate") strings together.

- Input is always read as a string.
- We use `Scanner` tool for reading input.
- This tool can be imported using `import java.util.Scanner;` before the beginning of the main program's frame.
- The tool itself is created with `Scanner scanner = new Scanner(System.in);`
- `scanner` tool's `nextLine()` method used to read input.
- When user writes something and presses enter, the provided string is assigned to a **string variable**.

##### Fundamentals of Strings
- "String" more like "string of characters".

##### Concatenation - Joining Strings Together
- Multiple strings can be joined using the `+` operator. 
