C Lexical Analyzer (Lexer)

Project Overview

This project implements a lexical analyzer in C that reads a source-code file, scans its contents, identifies tokens, and classifies them into categories. These categories include keywords, identifiers, numeric literals, character literals, string literals, operators, special characters, and preprocessor directives.

The lexer also performs basic lexical error checking, including invalid numeric literals, unclosed character or string literals, and unmatched brackets. It demonstrates how the lexical analysis phase of a compiler processes source code.

Features

- Reads C source code from an input file.
- Identifies C keywords and identifiers.
- Recognizes decimal, floating-point, hexadecimal, octal, and binary-style numeric literals.
- Detects character and string literals.
- Identifies operators and special characters.
- Displays preprocessor lines.
- Reports certain lexical errors and unmatched brackets.
- Tracks line numbers for error reporting.

Technologies Used

- C Programming
- File Handling
- Character Processing
- String Handling
- GCC Compiler
- Linux Environment

Project Architecture

The project uses separate source and header files to organize token recognition and source-file scanning.

- Token recognition: Checks keywords, identifiers, and numeric literal formats.
- Source scanning: Reads the input file character by character, identifies token boundaries, and displays classifications.
- Header declarations: Provides function declarations and shared includes.
- Main function: Accepts the input filename as a command-line argument and starts lexical analysis.

How It Works

1. The program receives the source-code filename through a command-line argument.
2. It opens the file for reading.
3. It scans characters and groups them into possible tokens.
4. It classifies each token using recognition functions.
5. It prints the token category and value.
6. It reports supported lexical errors and checks for unmatched brackets.
7. It closes the input file.

Compilation

Open a terminal in the project directory and compile the required source files:

gcc main.c lexer.c -o lexer

The main source includes the scanning implementation directly, so "read.c" should not also be passed separately in this compilation command.

Execution

Run the program by providing a C source file as an argument:

./lexer test.c

Replace "test.c" with the path to the source file you want to analyze.

Learning Outcomes

- Understanding lexical analysis and token classification.
- Practicing C file handling and character-by-character scanning.
- Using functions to recognize different token types.
- Understanding command-line arguments.
- Implementing basic lexical error detection.
- Learning how a lexer contributes to compiler design.

Future Improvements

- Improve handling of comments and escape sequences.
- Support more complete C operator and token rules.
- Strengthen identifier and numeric-literal validation.
- Improve line-number tracking and error messages.
- Handle longer tokens safely using dynamic storage or bounds checking.

Author

Raj Chilshetty
