==============================================================================
Declarative Language Definition
==============================================================================

Notes on a general approach to declarative language definition. The goal is to separate the concerns of language definition from language implementation. A language definition states the specific rules for a language. Language implementations typically have much in common. By factoring out the language-specific rules into a declarative meta-language, the language-independent aspects of implementations can be automatically generated.

A Language Designer's Workbench
-------------------------------------------------------------------------------

- Objective: A workbench supporting design and implementation of programming languages

- Approach: Declarative multi-purpose domain-specific meta-languages

- Meta-Languages: Languages for defining languages

- Domain-Specific: Linguistic abstractions for domain of language definition (syntax, names, types, …)

- Multi-Purpose: Derivation of interpreters, compilers, rich editors, documentation, and verification from single source

- Declarative: Focus on what not how; avoid bias to particular purpose in language definition


Meta-Language Design
-------------------------------------------------------------------------------

Representation

- Standardized representation for <aspect> of programs
- Independent of specific object language

Specification Formalism

- Language-specific declarative rules
- Abstract from implementation concerns

Language-Independent Interpretation

- Formalism interpreted by language-independent algorithm
- Multiple interpretations for different purposes
- Reuse between implementations of different languages
