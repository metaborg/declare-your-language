To Do
-------------------------------------------------------------------------------

demonstrate how ambiguity is shown (amb nodes)

How layout is treated

motivate the need for (lexical) disambiguation and how that is treated in other (scanner based) approaches

Generated formatting rules

Completion

demonstrate pretty-printing with builder for boxes

Grammar normalization

Demo of testing syntax

illustrate use of BNF

motivate need for EBNF by showing encoding of lists in BNF

consider dropping the explanation of BNF and EBNF dialects; explain everything in terms of SDF (subsets); start with plain context-free grammars; motivate why that is not sufficient / convenient

refer to other formalisms for syntax definition

Talk about modeling syntax to get clean AST structure


Layout constraints

empty syntax: production for brackets

Language Composition and operations on languages

https://en.wikipedia.org/wiki/Formal_language

Language
-------------------------------------------------------------------------------

| Language is a purely human and non-instinctive method of communicating ideas, emotions, and desires by means of a system of voluntarily produced symbols.

Edward Sapir: Language. An Introduction to the Study of Speech.



Syntax
-------------------------------------------------------------------------------

syntax is the form of


definition of syntax is typically done in terms of parsing

we take a declarative approach to syntax definition

Noam Chomsky

Generation of sentences instead of recognition


Context-free Grammars
-------------------------------------------------------------------------------



Abstract Syntax Constructors
-------------------------------------------------------------------------------

Spoofax uses SDF3 to generate parsers that transform text to ATerms. Stratego strategies transform ATerms to ATerms.

Each context-free syntax production in SDF3 determines how to form ATerms from the ATerms produced by parsing the nonterminals in the RHS. There are 3 cases:

1. Explicit constructor

- The specified constructor is used to form the ATerm.

2. Chain production with no explicit constructor

- The ATerm is the same as that produced by RHS.

3. Non-chain production with no explicit constructor

- Not supported?




Regular Expressions
-------------------------------------------------------------------------------


Ambiguities
-------------------------------------------------------------------------------


Grammar Transformation
-------------------------------------------------------------------------------


Declarative Disambiguation
-------------------------------------------------------------------------------

associativity, priority (precedence)


Lexical Syntax
-------------------------------------------------------------------------------

regular grammars


-------------------------------------------------------------------------------


Lexical Disambiguation
-------------------------------------------------------------------------------


Layout
-------------------------------------------------------------------------------


Layout Constraints
-------------------------------------------------------------------------------


Other Syntax Definition Formalisms
-------------------------------------------------------------------------------

In this chapter we have used SDF3 notation for syntax definition. There are many other grammar formalisms that use a variation of the syntax used here.

- BNF
- EBNF
- ANTLR
- Xtext
- Rascal


Exercises
-------------------------------------------------------------------------------

* Show reduction sequence for a sentence given a grammar
