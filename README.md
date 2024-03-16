# cmpsc461-proj1-parser

Introduction
This project provides hands-on experience with lexical analysis and abstract syntax tree (AST) construction,
fundamental concepts in compiler construction and programming languages.
Instructions
1. You must submit file name as project1 parser.py. Any other file name will not be accepted by the
GradeScope’s autograder. Please strictly adhere to this format.
2. You must implement Lexer, Parser classes, and implement the parse function in the Parser class
along with related functions.
3. Please generate your AST in the canonical form; refer to the example given in test utility.py.
Failure to comply will result in rejection of your submission by GradeScope.
4. You are advised to use git for maintaining your code changes throughout Project 1 and 2. There are
many online tutorials available for git.
5. Please refer to grammar.txt, example.txt, and test utility.py before beginning the project to
understand the expected output format and the test cases.
6. If you get stuck, please reach out early. Do not wait until the last moment.
Grammar
Please refer to the grammar.txt in the project folder.
Example
Refer to example.txt for an example. A statement in the language x = 5 + 3 matches the following

Grammar rule:
1. expression -> variable ’=’ arithmetic expression.
2. arithmetic expression -> term ((’+’ | ’-’) term) *
3. term -> factor ((’*’ | ’/’) factor) *
4. factor -> number

Implementation
The file project1 parser.py contains lexer and parser classes and a few functions as guidelines for struc-
turing your project. We highly encourage you to implement all those functions. If you decide to come up
with your own implementation, please ensure you follow the below restrictions:
1. You must implement the parse function declared in the parser class in project1 parser.py. The
checker will invoke the parse function to retrieve the AST representation of the program code to
verify correctness.
2. Your output must match the pre-order traversal of the AST for each statement in the programming
language. Please review the comment in test utility.py before writing any code
