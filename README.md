# Low Level Embeded C

# Low Lvevel Embeded About 

- This repository is one of the several tracks that I'm learning to become a Embeded Linux Developer at my hobbies and below is a tree diagram of all files of what I've been working on:

# General
* Why C programming is awesome 
+ Who invented C
* Who are Dennis Ritchie, Brian Kernighan and Linus Torvalds
* What happens when you type gcc main.c
* What is an entry point
* What is main
* How to print text using printf, puts and putchar
* How to get the size of a specific type using the unary operator sizeof
* How to compile using gcc
* What is the default program name when compiling with gcc
* What is the official Holberton C coding style and how to check your code with betty-style
* How to find the right header to include in your source code when using a standard library function
* How does the main function influence the return value of the program
## Requirements C
* Allowed editors: vi, vim, emacs
* All your files will be compiled on Ubuntu 14.04 LTS using gcc 4.8.4
* All your files should end with a new line
* A README.md file at the root of the holbertonschool-low_level_programming repo, containing a description of the repository
* A README.md file, at the root of the folder of this project, containing a description of the project
* There should be no errors and no warnings during compilation
* You are not allowed to use system
* Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
# 0-preprocessor: Preprocessor
*A script that runs a C file through the preprocessor and save the result into another file. The C file name will be saved in the variable $CFILE; The output should be saved in the file c using gcc $CFILE -E -o c.*

# 1-compiler: Compiler
A script that compiles a C file but does not link. The C file name will be saved in the variable $CFILE; The output file should be named the same as the C file, but with the extension .o instead of .c;

Example: if the C file is main.c, the output file should be main.o using gcc -c $CFILE.

# 2-assembler: Assembler
A script that generates the assembly code of a C code and save it in an output file. The C file name will be saved in the variable $CFILE; The output file should be named the same as the C file, but with the extension .s instead of .c.

Example: if the C file is main.c, the output file should be main.s using gcc -S $CFILE.

# 3-name: Name
A script that compiles a C file and creates an executable named cisfun. The C file name will be saved in the variable $CFILE using gcc $CFILE -o cisfun.

# 4-puts.c: Hello, puts
A C program that prints exactly "Programming is like building a multilingual puzzle, followed by a new line.. Use the function puts; You are not allowed to use printf; Your program should end with the value 0 using:

#include <stdio.h>
```
int main(void) { puts("Programming is like building a multilingual puzzle\n"); return (0); }
```
# 5-printf.c: Hello, printf
A C program that prints exactly with proper grammar, but the outcome is a piece of art,, followed by a new line. Use the function printf; You are not allowed to use the function puts; Your program should return 0; Your program should compile without warning when using the -Wall gcc option using:

{ #include <stdio.h>
```
int main(void) { printf("with proper grammar, but the outcome is a piece of art,\n"); return (0); } }
```
# 6-size.c: Size is not grandeur, and territory does not make a nation
A C program that prints the size of various types on the computer it is compiled and run on. You should produce the exact same output as in the example; Warnings are allowed; Your program should return 0; You might have to install the package libc6-dev-i386 on your Linux (Vagrant) to test the -m32 gcc option using:

{ #include <stdio.h>
```
int main(void) { int a; long int b; long long int c; char d; float f;
```
*[printf("Size of a char: %lu byte(s)\n", (unsigned long)sizeof(d));
printf("Size of an int: %lu byte(s)\n", (unsigned long)sizeof(a));
printf("Size of a long int: %lu byte(s)\n", (unsigned long)sizeof(b));
printf("Size of a long long int: %lu byte(s)\n", (unsigned long)sizeof(c));
printf("Size of a float: %lu byte(s)\n", (unsigned long)sizeof(f));
return (0);
} }](https://www.programiz.com/c-programming/examples/sizeof-operator-example)*

# 100-intel: Intel
A script that generates the assembly code (Intel syntax) of a C code and save it in an output file. The C file name will be saved in the variable $CFILE. The output file should be named the same as the C file, but with the extension .s instead of .c.

Example: if the C file is main.c, the output file should be main.s using gcc -S -masm=intel $CFILE.

# 101-quote.c: UNIX is basically a simple operating system, but you have to be a genius to understand the simplicity
A C program that prints exactly and that piece of art is useful" - Dora Korpar, 2015-10-19, followed by a new line, to the standard error. You are not allowed to use any functions listed in the NAME section of the man (3) printf or man (3) puts; Your program should return 1; Your program should compile without any warnings when using the -Wall gcc option using:

{ #include <stdio.h>
```
int main(void) { write(2, "and that piece of art is useful" - Dora Korpar, 2015-10-19\n", 61);
```
```
return (1);
 
```
} }

---
## Table of Contents : open file folder

- 1. [0x00. C - Hello, World](./0x00-hello_world)

- 2. [0x01. C - Variables, if, else, while](./0x01-variables_if_else_while)

- 3. [0x02. C - Functions, nested loops](./0x02-functions_nested_loops)

- 4. [0x03. C - More functions, more nested loops](./0x03-more_functions_nested_loops)

- 5. [0x04. C - Pointers, arrays and strings](./0x04-pointers_arrays_strings)

- 6. [0x05. C - More pointers, arrays and strings](./0x05-pointers_arrays_strings)

- 7. [0x06. C - Even more pointers, arrays and strings](./0x06-pointers_arrays_strings)

- 8. [0x07. C - Even more, more pointers, arrays and strings](./0x07-pointers_arrays_strings)

- 9. [0x08. C - Recursion](./0x08-recursion)

- 10. [0x09. C - Static libraries](./0x09-static_libraries)

- 11. [0x0A C -  Argc, Argv](./0x0A-argc_argv)

- 12. [0x0B. C - Malloc, Free](./0x0B-malloc_free)

- 13. [0x0C. C - More malloc, free](./0x0C-more_malloc_free)

- 14. [0x0D. C - Preprocessor](./0x0D-preprocessor)

- 15. [0x0E. C - Structures, typedef](./0x0E-structures_typedef)

- 16. [0x0F. C - Function pointers](./0x0F-function_pointers)

- 17. [0x10. C - Variadic functions](./0x10-variadic_functions)

- 18. [0x12. C - Singly linked lists](./0x12-singly_linked_lists)

- 19. [0x13. C - More singly linked lists](./0x13-more_singly_linked_lists)

- 20. [0x14. C - Bit manipulation](./0x14-bit_manipulation)

- 21. [0x15. C - File I/O](./0x15-file_io)

- 22. [0x17. C - Doubly linked lists](./0x17-doubly_linked_lists)

- 23. [0x18. C - Dynamic libraries](./0x18-dynamic_libraries)

- 24. [0x19. C - Stacks, Queues - LIFO, FIFO](./0x19-stacks_queues_lifo_fifo)

- 25. [0x1C. C - Makefiles](./0x1C-makefiles)

- 26. [0x1E  C - Search Algorithms](./0x1E-search_algorithms)
---



# Author 
   - All files is maintained and owned by Maririn312
