# ft_printf
ft_printf - 42 School Project
Overview
ft_printf is a project from the 42 School curriculum that involves recreating a simplified version of the C standard library's printf function. This project aims to deepen understanding of variadic functions, string manipulation, and low-level formatting in C. The goal is to implement a custom ft_printf function that mimics the behavior of the original printf for specific format specifiers, handling various data types and formatting options.
Project Description
The ft_printf function is designed to parse a format string and handle various format specifiers, such as:

%c: Character
%s: String
%d/%i: Integer
%u: Unsigned integer
%x/%X: Hexadecimal (lowercase/uppercase)
%p: Pointer address
%%: Literal percent sign

Additional features may include handling flags, width, and precision (depending on the project requirements). The implementation uses variadic functions (va_list, va_arg, etc.) to process variable arguments and custom string manipulation to format output.
Features

Supports basic format specifiers as required by the 42 project guidelines.
Handles variable arguments using the C standard library's variadic functions.
Outputs formatted strings to the standard output (file descriptor 1).
Adheres to 42 School's Norminette coding standards.

Getting Started
Prerequisites

A C compiler (e.g., gcc or clang)
make for using the provided Makefile
Basic understanding of C programming and variadic functions

Compilation
To compile the project, run:
make

This generates the ft_printf.a static library (or an executable if a main.c is provided). To clean up object files or the library, use:
make clean
make fclean

Usage
To use ft_printf in your own project:

Include the header file:
#include "ft_printf.h"


Link the ft_printf.a library during compilation.

Call the function like the standard printf:
ft_printf("Hello, %s! You are %d years old.\n", "Alice", 25);



For testing, you can compile with the provided main.c (if included):
gcc main.c src/ft_printf.c -Iinclude
./a.out

Learning Outcomes
Through this project, I have gained experience in:

Implementing variadic functions in C
Parsing and processing format strings
Managing string manipulation and memory efficiently
Debugging complex string output issues
Most importantly improved my problem solving skills

Notes

The implementation is designed to be efficient and robust, handling edge cases as specified in the project guidelines.
The code has been tested against the 42 School's evaluation criteria (e.g., Moulinette or custom testers like printfTester).
Feel free to explore the source code to understand the implementation details!
