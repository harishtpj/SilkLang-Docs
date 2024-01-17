---
description: Welcome to the Silk programming language!
---

# The Silk Programming Language

SilkLang is a programming language created for **simple** usage but packed with **advanced** features. This programming language is intended for educational use, as mastering this language would make the learners easier to enter the arena of computer programming. Also, the programming language is made in such a way that it can be **Platform Independent.** Silk is still in its early stages, so the language is still changing rapidly. Nonetheless, we’re trying our best to keep the guide and the documentation as up to date as possible.

## Installation

If you haven't installed Silk, head over to the project's [README](https://github.com/harishtpj/SilkLang/tree/master?tab=readme-ov-file#installation) for more information.

## Quick tour of the language

The Silk interpreter has two modes:

1. The **REPL** mode: The famous **R**ead **E**val **P**rint **L**oop mode. This Opens up an interactive session in which you can execute simple commands.
2. The **Execution** mode: You'll pass an `.slk` file to the interpreter, and it will be interpreted.

For simple programs, the REPL mode is enough. But if you want to use the language for complex tasks, you need to use the interpreter.

## The REPL mode

To start the REPL, run

```
$ silk
```

You'll be greeted with the following message

```
The Silk programming language REPL v1.0.0
Copyright (c) 2024, Harish Kumar

Silk .>> 
```

You can execute various commands within this mode:

```
Silk .>> println "Hello, REPL";
Hello, REPL
```

By default, the result of expressions are not shown in the interpreter. Just exclude the semicolon to view the result

```
Silk .>> 3 + 2;
Silk .>> 3 + 2
:= 5
```

## The Execution mode

For simple programs, the REPL is good enough. But if you want to write large programs,  the execution mode is best. Most of the time, this mode is used

Let's assume that you need to get input from the user and greet him/her with a message. To implement it, you need to follow these steps:

* Create a `greet.slk` file and add the following content:&#x20;

```clike
# Simple program to greet user

let userName := input("Enter your name: ");
println fmt("Hello, %s! Hope you're fine.", userName);
```

* Having saved the file, run the following command:

```
$ silk greet.slk
```

* You'll see the following result

```
Enter your name: Harish
Hello, Harish! Hope you're fine.
```

🥳 Yay! You just ran your first Silk program.
