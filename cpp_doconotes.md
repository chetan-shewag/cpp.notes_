# C++ LANGUAGE
---
- Our Cpp tutoril provides you knowlwdge of Cpp form basic to scartch.
- We make seperet part for sepret topic,with example.
- We gave you an example with its berif descripition.

Introduction

# 1. COMPILIER

# Compilier
---
There are some tools which you neend regarding this tutorial.
- COMPUTER
- COMPILER

C++ is the language which develop year over year, and our tutorial provides you the most modified versioin of the C++ Language. The current compier which we used is modified as the our C++11 means the featues introduced by the 2011 standered.



# - WHAT IS COMPILER?
---
---
Computer understands only one langugage which contains the set of instruction made up of zeros and ones, this language is called as the **binary language** as well as we also say it **machine langugae**

A single instruction of computer look like this

| oooo | 1000101 |

A particular computer's machine language program that allows a user to input two numbers, adds the two numbers together, and displays the total could include these machine code instructions:

| 00000 | 10011110 |

| 00001 | 11110100 |

| 00010 | 10011110 |

| 00011 | 11010100 |

| 00100 | 10111111 |

| 00101 | 00000000 |


As you can imagine, programming a computer directly in machine language using only ones and zeros is very hard to learn this binary language.To make programming easier, high level languages have been developed. High level programs also make it easier for programmers to inspect and understand each other's programs easier.

This is a portion of code written in C++ that accomplishes the exact same purpose:

```
{
1 int a, b, sum;
2 cin >> a;
3 cin >> b;
4             
5 sum = a + b;
6 cout << sum << endl; 
}
```

Even if you cannot really understand the code above, you should be able to appreciate how much easier it will be to program in the C++ language as opposed to machine language.

Because a computer can only understand machine language and humans wish to write in high level languages high level languages have to be re-written (translated) into machine language at some point. This is done by special programs called compilers, interpreters, or assemblers that are built into the various programming applications.

C++ is designed to be a compiled language, meaning that it is generally translated into machine language that can be understood directly by the system, making the generated program highly efficient. For that, a set of tools are needed, known as the development toolchain, whose core are a compiler and its linker.

- console program
---
Console programs are programs that use text to communicate with the user and the environment, such as printing text to the screen or reading input from a keyboard.

Console programs are easy to interact with, and generally have a predictable behavior that is identical across all platforms. They are also simple to implement and thus are very useful to learn the basics of a programming language: The examples in these tutorials are all console programs.


The way to compile console programs depends on the particular tool we were using.

The easiest way for beginners to compile C++ programs is by using an Integrated Development Environment (IDE). An IDE generally integrates several development tools, including a text editor and tools to compile programs directly from it.
 
Here you have instructions on how to compile and run console programs using different free Integrated Development Interfaces (IDEs):

# - what is IDE?
That was an a pletform were we can run and make our program and check either there is some erroe or not and IDE provide us to some compiler 
compier only work on IDE , what we wote on the IDE that compiles with the help of comiler then complie it into a **binray language**

- IDE WHICH WE USE IT WAS VS STUDIO
[vs studio](https://cplusplus.com/doc/tutorial/introduction/visualstudio/)



---
---
---
---
---
---
---







Basic of C++
# Structure of program
---
The best way to learn a programming language is by writing programs. Typically, the first program beginners write is a program called "Hello World", which simply prints "Hello World" to your computer screen. Although it is very simple, it contains all the fundamental components C++ programs have:

```
{
    // my first program in C++
#include <iostream>

int main()
{
  std::cout << "Hello World!";
}
}
```

**output**
Hello World!

In between the line number 107 to 117 shows the C++ code for this program. and the line number 119 and 120 shows the result when the program is executed by a computer.The line number 109 are line numbers to make discussing programs and researching errors easier. That is not the part of the program.

- **let explain this program line by line**

- Line 109 : **// my first program in C++**
Two slash signs indicate that the rest of the line is a comment inserted by the programmer but which has no effect on the behavior of the program. Programmers use them to include short explanations or observations concerning the code or program. In this case, it is a brief introductory description of the program.

- Line 110 : #include <iostream>
Lines beginning with a hash sign (#) are directives read and interpreted by what is known as the preprocessor. They are special lines interpreted before the compilation of the program itself begins. In this case, the directive #include <iostream>, instructs the preprocessor to include a section of standard C++ code, known as header iostream, that allows to perform standard input and output operations, such as writing the output of this program (Hello World) to the screen.

- Line 111: **A blank line.**
Blank lines have no effect on a program. They simply improve readability of the code.

- Line 112: **int main ()**
This line take action on the declaration of a function. Essentially, a function is a group of code statements which are given a name: in this case, this gives the name "main" to the group of code statements that follow. Functions will be discussed in detail in a later chapter, but essentially, their definition is introduced with a succession of a type (int), a name (main) and a pair of parentheses (()), optionally including parameters.

The function named main is a special function in all C++ programs; it is the function called when the program is run. The execution of all C++ programs begins with the main function, regardless of where the function is actually located within the code.


- Line 113 and 115: **{ and }**
The open brace ({) at line 113 indicates the beginning of main's function definition, and the closing brace (}) at line 115, indicates its end. Everything between these braces is the function's body that defines what happens when main is called. All functions use braces to indicate the beginning and end of their definitions.

- Line 114: **std::cout << "Hello World!";**
This line is a C++ statement. A statement is an expression that can actually produce some effect. It is the meat of a program, specifying its actual behavior. Statements are executed in the same order that they appear within a function's body.

This statement has three parts: First, std::cout, which identifies the standard character output device (usually, this is the computer screen). Second, the insertion operator (<<), which indicates that what follows is inserted into std::cout. Finally, a sentence within quotes ("Hello world!"), is the content inserted into the standard output.

Notice that the statement ends with a semicolon (;). This character marks the end of the statement, just as the period ends a sentence in English. All C++ statements must end with a semicolon character. One of the most common syntax errors in C++ is forgetting to end a statement with a semicolon.

You may have noticed that not all the lines of this program perform actions when the code is executed. There is a line containing a comment (beginning with //). There is a line with a directive for the preprocessor (beginning with #). There is a line that defines a function (in this case, the main function). And, finally, a line with a statements ending with a semicolon (the insertion into cout), which was within the block delimited by the braces ( { } ) of the main function.


The program has been structured in different lines and properly indented, in order to make it easier to understand for the humans reading it. But C++ does not have strict rules on indentation or on how to split instructions in different lines. For example, instead of

```
1.    int main ()
2.{
3. std::cout << " Hello World!";
4.}
```

```
We could have written:
1.int main () { std::cout << "Hello World!"; }
```
all in a single line, and this would have had exactly the same meaning as the preceding code.

In C++, the separation between statements is specified with an ending semicolon (;), with the separation into different lines not mattering at all for this purpose. Many statements can be written in a single line, or each statement can be in its own line. The division of code in different lines serves only to make it more legible and schematic for the humans that may read it, but has no effect on the actual behavior of the program.

 **Now, let's add an additional statement to our first program:**

```
// my second program in C++
#include <iostream>

int main ()
{
  std::cout << "Hello World! ";
  std::cout << "I'm a C++ program";
}
 ```

 **output**=Hello world! I'm a C++ program


In this case, the program performed two insertions into std::cout in two different statements. Once again, the separation in different lines of code simply gives greater readability to the program, since main could have been perfectly valid defined in this way:

```
int main () { std::cout << " Hello World! "; std::cout << " I'm a C++ program "; }
```
The source code could have also been divided into more code lines instead:
```
int main ()
{
  std::cout <<
    "Hello World!";
  std::cout
    << "I'm a C++ program";
}
```
And the result would again have been exactly the same as in the previous examples.

Preprocessor directives (those that begin by #) are out of this general rule since they are not statements. They are lines read and processed by the preprocessor before proper compilation begins. Preprocessor directives must be specified in their own line and, because they are not statements, do not have to end with a semicolon (;).


- # Comments
---
As noted above, comments do not affect the operation of the program; however, they provide an important tool to document directly within the source code what the program does and how it operates.

C++ supports two ways of commenting code:

- // line comment
- /* block comment */

The first of them, known as **line comment**, discards everything from where the pair of slash signs (//) are found up to the end of that same line. The second one, known as **block comment**, discards everything between the /* characters and the first appearance of the */ characters, with the possibility of including multiple lines.

**Let's add comments to our second program:**
```
/* my second program in C++
   with more comments */

#include <iostream>

int main ()
{
  std::cout << "Hello World! ";     // prints Hello World!
  std::cout << "I'm a C++ program"; // prints I'm a C++ program
}
Hello World! I'm a C++ program

```

**output**=Hello World! I'm a C++ program

If comments are included within the source code of a program without using the comment characters combinations //, /* or */, the compiler takes them as if they were C++ expressions, most likely causing the compilation to fail with one, or several, error messages.

- # Using namespace std:
---
If you have seen C++ code before, you may have seen cout being used instead of std::cout. Both name the same object: the first one uses its unqualified name (cout), while the second qualifies it directly within the namespace std (as std::cout).

cout is part of the standard library, and all the elements in the standard C++ library are declared within what is called a namespace: the namespace std.

In order to refer to the elements in the std namespace a program shall either qualify each and every use of elements of the library (as we have done by prefixing cout with std::), or introduce visibility of its components. The most typical way to introduce visibility of these components is by means of using declarations:


- **using namespace std;**

The above declaration allows all elements in the std namespace to be accessed in an unqualified manner (without the std:: prefix).

With this in mind, the last example can be rewritten to make unqualified uses of cout as:


```
// my second program in C++
#include <iostream>
using namespace std;

int main ()
{
  cout << "Hello World! ";
  cout << "I'm a C++ program";
}
```

**outout**=Hello World! I'm a C++ program

Both ways of accessing the elements of the std namespace (explicit qualification and **using**declarations) are valid in C++ and produce the exact same behavior. For simplicity, and to improve readability, the examples in these tutorials will more often use this latter approach with **using**declarations, although note that **explicit qualification** is the only way to guarantee that name collisions never happen.

---