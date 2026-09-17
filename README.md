# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```c
#include <stdio.h>

int main()
{
    int age = 20;
    float mark = 85.5;
    char grade = 'A';
    char name[] = "Ranjani";

    printf("Integer Literal: %d\n", age);
    printf("Float Literal: %.1f\n", mark);
    printf("Character Literal: %c\n", grade);
    printf("String Literal: %s\n", name);

    return 0;
}

```
# Output:

<img width="1262" height="480" alt="image" src="https://github.com/user-attachments/assets/6dddd652-98dc-45d8-b773-4f887a57064e" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```c
#include <stdio.h>

#define PI 3.14

int main()
{
    const int MAX = 100;

    printf("Macro Constant PI = %.2f\n", PI);
    printf("Constant Variable MAX = %d\n", MAX);

    return 0;
}

```
# Output:

<img width="1181" height="425" alt="image" src="https://github.com/user-attachments/assets/c14e4a95-3a9e-43ea-b978-865b08d89701" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```c
#include <stdio.h>

int main()
{
    int a = 10;
    float b = 20.5f;
    double c = 30.12345;
    char d = 'A';

    printf("Integer: %d\n", a);
    printf("Float: %.2f\n", b);
    printf("Double: %.5lf\n", c);
    printf("Character: %c\n", d);

    return 0;
}

```
# Output:

<img width="1141" height="438" alt="image" src="https://github.com/user-attachments/assets/f935c0f4-12b3-48c5-a57f-a64a99c07c2b" />

# Result: 
Thus, the C program successfully demonstrates int, float, double, and char data types.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```c
#include <stdio.h>

int main()
{
    int a, b;

    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    printf("\nArithmetic Operations:\n");
    printf("Addition = %d\n", a + b);
    printf("Subtraction = %d\n", a - b);
    printf("Multiplication = %d\n", a * b);
    printf("Division = %d\n", a / b);
    printf("Remainder = %d\n", a % b);

    printf("\nBitwise Operations:\n");
    printf("AND = %d\n", a & b);
    printf("OR = %d\n", a | b);
    printf("XOR = %d\n", a ^ b);
    printf("Left Shift = %d\n", a << 1);
    printf("Right Shift = %d\n", a >> 1);
    printf("NOT = %d\n", ~a);

    return 0;
}

```
# Output:

<img width="1362" height="687" alt="image" src="https://github.com/user-attachments/assets/8ba4233a-27b5-42a8-ac5d-db49f1d80fbd" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```c
#include <stdio.h>
#include <ctype.h>

int main()
{
    char ch;

    printf("Enter a character: ");
    scanf("%c", &ch);

    printf("%s\n",
        isdigit(ch) ? "Digit" :
        (isalpha(ch) ?
            (ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||
             ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'
             ? "Vowel" : "Consonant")
            : "Special Symbol"));

    return 0;
}

```
# Output:
<img width="1176" height="558" alt="image" src="https://github.com/user-attachments/assets/76faee73-e011-4fbb-99f7-e1e0bb642ec9" />
<img width="1162" height="553" alt="image" src="https://github.com/user-attachments/assets/b8ae8c73-bb10-45f4-bd78-d51f4269b7ae" />
<img width="1331" height="555" alt="image" src="https://github.com/user-attachments/assets/abf2d7d0-8591-4338-8a43-3d42d9efc959" />
<img width="1155" height="551" alt="image" src="https://github.com/user-attachments/assets/3d3b4408-c149-4cf6-baa0-686677d5c108" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


