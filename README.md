# Interpreter in Go

A simple interpreter for the Monkey programming language, written in Go, based on Thorsten Ball’s book [*How to Write an Interpreter in Go*](https://interpreterbook.com/).

## 📚 About

This project implements a fully working interpreter for a Lisp-like language called **Monkey**, as described in the book. It's built from scratch using idiomatic Go and includes all major components of an interpreter:

- A **lexer** that tokenizes the source code  
- A **Pratt parser** to generate the abstract syntax tree (AST)  
- An **evaluator** that walks the AST and executes the code  
- A basic **object system** (integers, booleans, strings, functions, closures)  
- Support for **let-bindings**, **conditionals**, **first-class functions**, and a **REPL**

## 🧠 Learning Goals

This project is a great foundation for understanding:

- Lexing and parsing theory
- Interpreter architecture
- Scope and closures
- Functional programming concepts in a small language
  
## 🚀 Features

- REPL for interactive programming  
- Lexical scoping and closures  
- Built-in functions (e.g., `len`, `first`, `last`, `push`, etc.)  
- Error handling and runtime type checking  

## 🛠️ Getting Started

### Prerequisites

- [Go](https://golang.org/dl/) (version 1.18+ recommended)

### Clone and Run

```bash
git clone https://github.com/your-username/monkey-interpreter.git
cd monkey-interpreter
go run main.go

## 🧪 REPL Example

```text
>> let add = fn(a, b) { a + b; };
>> add(2, 3);
5
>> let twice = fn(f, x) { f(f(x)); };
>> twice(fn(x) { x + 1; }, 5);
7


