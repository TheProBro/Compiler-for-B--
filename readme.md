# B-- Toy Language

B-- is a simple toy language implemented using Lex and Yacc. It supports basic programming constructs and operations.

## Contributors

- Abhishek Jaiswal
- Devanshu Dhawan

## Lexical Analysis (Lex)

The Lex file defines the lexical rules for tokenizing the input source code. It defines various tokens used in the B-- language, including keywords, operators, identifiers, and literals. The tokens recognized by Lex include:

- Whitespace: Skips whitespace characters.
- Newline: Represents a newline character.
- Tab: Represents a tab character.
- Float: Matches floating-point numbers.
- Int: Matches integer numbers.
- String: Matches string literals.
- IF, THEN, FOR, TO, STEP, DIM, DATA, GOTO, GOSUB, RETURN, DEF, LET, INPUT, PRINT, REM, END: Keywords in B--.
- NEQ, LE, GE, EQ, LT, GT: Comparison operators.
- PLUS, MINUS, MUL, DIV, POW: Arithmetic operators.
- COMMA, SEMICOLON, L_BRACE, R_BRACE: Miscellaneous symbols.
- EXCLAMATION: Represents the exclamation mark.
- FN: Matches function names.
- DOLLAR: Represents the dollar sign.
- MODULO: Represents the modulo operator.
- HASH: Represents the hash symbol.
- IDENTIFIER: Matches identifiers (variable names).
- Unexpected character: Prints an error message for unexpected characters.

## Syntax Analysis (Yacc)

The Yacc file defines the syntax rules for parsing the input source code based on the tokens generated by Lex. It specifies the grammar for the B-- language. The supported syntax includes statements, expressions, control structures, input/output operations, and more.

The B-- language supports the following constructs:

- Data statements: Used for declaring data values.
- Def statements: Used for defining functions.
- Dim statements: Used for declaring arrays.
- End statements: Marks the end of the program.
- For statements: Used for loop constructs.
- Gosub statements: Transfers control to a subroutine.
- Goto statements: Transfers control to a specific line number.
- If statements: Used for conditional branching.
- Let statements: Used for variable assignments.
- Input statements: Reads input from the user.
- Print statements: Prints output to the console.
- Rem statements: Comments or remarks.
- Return statements: Returns from a subroutine or function.


## How to Run

To run the B-- toy language, follow these steps:

1. Install Lex and Yacc on your system.
2. Clone the B-- repository: `git clone https://github.com/Jaiswal0786/b--`.
3. Navigate to the project directory: `cd b--`.
4. Build the Lex and Yacc files: `lex b--_lex.l && yacc -d b--_yacc.y`.
5. Compile the generated C files: `gcc lex.yy.c y.tab.c -o b--`.
6. Run the B-- toy language: `./b--`.


Please note that the code for the B-- language implementation is not included in this README file. This file serves as a reference for understanding the language's features and syntax.
