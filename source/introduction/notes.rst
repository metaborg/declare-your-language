

Programming is expression of computational thinking
- expressing intention at right level of abstraction


- high-level vs low-level of abstraction

  - instructing computer
  - defining data structures and operations on them
  - solving a real world problem

- abstraction

  - DRY: don't repeat yourself
  - capture a bunch of operations in a new virtual operation
  - programming is abstracting: instructions denote what happens at run time

- abstraction mechanisms

  - procedural abstraction
  - functional abstraction
  - data abstraction

- linguistic abstraction

  - language support for abstraction
  - function definition and call
  - variable declaratin and use

- So: programming is instructing a computer


Compilers bridge the gap between high-level expression of intent and low-level machines.

Compiler construction is about translators: not just translators to machine/assembly code; it is about lowering a level or levels of abstraction

We can reapply these techniques of higher levels of abstraction



- separation of concerns




Aspects of language definition / phases of compiler
------------------------------------------------------------

- syntax
- static semantics
- dynamic semantics




Other Applications of Compiler Construction
------------------------------------------------------------

- even if you will not be developing traditional language, study of CC is useful

- HLL to MC is just one instantiation of compiler construction
- many compilers do not generate machine code (or machine code for a much higher-level virtual machine)
- domain-specific languages
- WebDSL to Java + HQL + JavaScript
- TypeScript to JavaScript
- SQL
- GreenMarl
- ...

Compiler as general design pattern to support linguistic abstraction

- Concrete compiler: translation from Mini-Java to bytecode
- Generalize: programming language to code for some target machine
- Generalize further: translation: language to other language
- General purpose programming languages
- Domain-specific languages
- Compilers/translaters appear everywhere in software engineering
- Linguistic abstraction

The role of Computer Science = commodify X (Frank Wood in PLDI keynote)



Compiler Correctness
----------------------------------------

- When is a compiler good?
- How do we know a compiler is correct?
- miscompilation
- how do we know a compiler miscompiles?
- semantics of programming language
- correctness with respect to specification

Dimensions of Compiler Design
----------------------------------------

- a compiler is a meta-program
- meta-program: program that operates on programs as data
- Compiling is just one kind of program processing
- there are many other kinds of meta-programs, i.e. other operations on programs as data

  - IDEs
  - editor services
  - completion
  - refactoring
  - bug finding
  - verification

- all these applications share compiler ingredients

- separate compilation
- incremental compilation

Interpreters vs Compilers
----------------------------------------

- phase separation not always so strict
- compiling at run-time
- just-in-time compilation
- interpreter: don't generate code, directly interpret abstract syntax tree

Compiler Implementation vs Language Definition
------------------------------------------------------------

- traditional focus in compiler construction on implementation
- correctness of compiler
- problem: miscompilation; how to avoid that? (see slides Xavier Leroy)
- separation of concerns: separate language definition from implementation of compiler components
- language workbenches: support that separation of concerns

we can apply compiler construction to itself by developing meta-languages for the high-level definition of aspects of language definition

- syntax definition
- static semantics definition
- dynamic semantics definition
- static analysis

- derive language implementation from language definition

From Compilers to Synthesizers
------------------------------------------------------------
Formal def of compiler

Behavior of program

Many possible realizations

Characteristic: staging of computation


Domain-Specific Languages
------------------------------------------------------------

DSL advantage: not dependendent on a specific implementation model

Domain analysis checklist
------------------------------------------------------------

- Domain Analysis
- What are the features of the domain?
- Language Design
- What are adequate linguistic abstractions?
- Coverage: can language express everything* in the domain?
- Minimality: but not more
- *) often the domain is unbounded; language design is making choice what to cover
- Semantics
- What is the semantics of such definitions?
- How can we verify the correctness / consistency of language definitions?
- Implementation
- How do we derive efficient language implementations from such definitions?




Declarative language definition
------------------------------------------------------------

- declarative: state what is the case, not what needs to be done
- automatic mapping to implementation


Why Study Compilers?
------------------------------------------------------------

- compilers define programming languages
- there are many kinds of compilers

Compiler as general design pattern to support linguistic abstraction
-----------------------------------------------------------------------

- Concrete compiler: translation from Mini-Java to bytecode
- Generalize: programming language to code for some target machine
- Generalize further: translation: language to other language
- General purpose programming languages
- Domain-specific languages
- Compilers/translaters appear everywhere in software engineering
- Linguistic abstraction

Language Workbenches
------------------------------------------------------------

next level of linguistic abstraction

meta-linguistic abstraction

History of language workbenches

The role of Computer Science = commodify X

commodity

Runtime System
------------------------------------------------------------

A compiler is an important part of the implementation of a programming language. However, the

- Programming Language = Compiler + Run-Time System

- Run-Time System

  - memory management / garbage collector
  - standard library
  - operating system




Programming Languages
----------------------------------------

Modern programming languages provide high-level abstractions that support

Programming languages

High-level Languages

- Procedural languages

  - C, Pascal

- Object-oriented languages

  - C++, Java, C#

- Functional languages

  - ML, Haskell, F#, Scala

- Dynamic languages

  - Scheme, Racket, Ruby, JavaScript, Dart, TypeScript

Low-level Languages

- Machine Code
  - instructions for a machine
  - physical machine: CPU/GPU

- virtual machine
- assembly code
- byte code


- linking


Don’t Repeat Yourself (DRY)
----------------------------------------

Don’t Repeat Yourself (DRY) principle to motivate language workbench and declarative meta-languages

In software engineering, the Don’t Repeat Yourself (DRY) principle means that “every piece of knowledge must have a single, unambiguous, authoritative representation within a system”

.. [PragProg] Andrew Hunt and David Thomas. 1999. The Pragmatic Programmer: From Journeyman to Master. Addison-Wesley Longman Publishing Co., Inc., Boston, MA, USA.
