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

#### Reading Strings

`reader.nextLine();` reads the user's input and *returns a string*

```java
//Create the tool for reading, assign it to variable classer scanner
Scanner scanner = new Scanner(System.in);
// String message = (user input)
String message = scanner.nextLine();
```

##### Program execution waits for input

- when the program's execution comes a statement that attempts to read input from the user, the execution stops and waits. `reader.nextLine();`

#### Variables

#### Learning objectives

- Understand the concept of a variable. You know what variable types, names, and values are.

- Know how to create and use string, integer, floating-point, and boolean variables.



- Variables can be used to store different types. This can be:
  
  1. text (String)
  
  2. whole numbers (int)
  
  3. floating-point numbers (double)
  
  4. true or false (boolean)

- A value can be assigned to the variables using =

- A variable's value can be joined to a string using the + sign.

- Variable names are unique - no two variables can have the same name.

- Once the variable name is declared, no need to declare the variable name again.

##### Changing a value assigned to a variable

- once the variable type has been declared, it can no longer be changed. 

- However, exceptions do exist: an integer can be assigned to a variable of the double type.

- Floating point value cannot be assigned to an in integer variable.

##### Naming variables

- Programming is a problem-solving tool.

- The aim is to create solutions for any given problem.

- The developer decides on the terms used to describe the problem domain.

- The terminology that is chosen, such as variable names, will serve to describe the problem for anyone who is to work with it in the future.

- Think about the concepts related to that problem and appropriate terms that could be used to describe them.

- If you find it hard to come up with relevant names, think of the ones that definitely do not describe it.

- After this, settle on some terminology that you're going to use.

- The good thing is, you can usually improve on it later on.

- Variable naming is limited by certain constraints. They are:
  
  1. Cannot contain special symbols, such as exclamation marks (!).
  
  2. Spaces are not allowed.
  
  3. Instead of spaces, the convention in java is to use a style known as **camelCase**. Note: the first letter of a variable name is always lower-cased.
  
  4. Numbers can be used in variable names, but the name should not being with a number.
  
  5. Names should not consists of only numbers.

- Permissible variable names:
  
  - lastDayOfMonth=20
  
  - firstYear=1952
  
  - name="Essi"

- Impermissible variable names:
  
  - last day of month=20
  
  - 1day=1952
  
  - beware!=1910
  
  - 1920=1

##### The type of the variable informs of possible values

| Type                                | Accepted values                                                                                        |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------ |
| Whole number, i.e., int             | An integer can contain whole numbers whose values lie between -2,147,483,648 and 2,147,483,648         |
| Floating-point number, i.e., double | Floating point numbers contains decimal numbers, with the greatest possible value being approx. 2^1023 |
| String                              | A string can contain text. Strings are enclosed in quotation marks.                                    |
| True or false values. i.e., boolean | A boolean contains either the value true or false.                                                     |

##### Reading different variable types from user

- In the text-based user interfaces, the user's input is always read as a string, since the user writes their input as text.

- We can read strings from the `input` command of the Scanner helper method.

- Other input types, such as integers, doubles, and booleans are also read as text. 

- They need to be converted to the target variable types using tools provided by java.

##### Reading integers

- The `Integer.valueOf` command converts a string to an integer.

- It takes the string containing the value to be converted as a parameter.

```java
String valueAsString = "42";
int value = Integer.valueOf(valueAsString);


System.out.println(value);
```

- When using a Scanner object, the reading of the value is usually inserted directly into the type of conversion.

```java
Scanner scanner = new Scanner(System.in);

int value = Integer.valueOf(scanner.nextLine());
```
