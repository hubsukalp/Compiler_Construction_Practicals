# Compiler Construction Lab

A collection of experiments and exercises for learning compiler construction using **Lex** and **Yacc**.

## Repository Overview

This repository contains practical experiments demonstrating core concepts of compiler design, including lexical analysis and syntax analysis. The main tools used are:

- **Lex** (Lexical Analyzer Generator) — Automates the process of tokenizing source code.
- **Yacc** (Yet Another Compiler Compiler) — Implements syntax analysis, parsing token streams produced by Lex.

## Language Composition

- **Lex:** 59.2%
- **Yacc:** 40.8%

## Getting Started

### Prerequisites

Make sure you have Lex and Yacc (or the equivalent implementations, commonly `flex` and `bison`) installed.

On Ubuntu/Debian systems:
```sh
sudo apt update
sudo apt install flex bison
```

### Running Experiments

Typical compilation steps:

1. **Compile the Lex file:**
   ```sh
   flex filename.l
   ```
2. **Compile the Yacc file:**
   ```sh
   bison -d filename.y
   ```
3. **Compile generated C files:**
   ```sh
   gcc lex.yy.c filename.tab.c -o parser
   ```
4. **Run the parser:**
   ```sh
   ./parser
   ```

_Note: Replace `filename.l` and `filename.y` with your actual file names._

## Lab Material

- [Compiler Construction Lab_T7478.pdf](https://github.com/user-attachments/files/22928259/Compiler.Construction.Lab_T7478.pdf)

This PDF contains detailed instructions and theory behind each experiment.

## Repository Structure

- `.l` files: Lex specifications for lexical analysis.
- `.y` files: Yacc specifications for syntax analysis.
- Additional C/C++ files may be present for extended functionality or testing.

## Author

**Sukalp Warhekar**  
ID: 22070521118

## License

This repository is for educational purposes.
