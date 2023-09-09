# Chapter 1: Introduction
## 1.1 Algorithms as opposed to programs
- algorithm: a finite sequence有限序列 of instructions, each of which has a clear meaning and can be performed with a finite amount of effort in a finite length of time
    - Imperative Programming: computation in terms of instructions that change the program/data state
    - Declarative Programming: the program should be accomplished without describing how to do it

- pseudocode: something that comes somewhere in between formatted English and computer program code, but is not runnable because certain details are ommitted省略.

## 1.2 Fundamental questions about algorithms
1. What is it supposed to do?
    - Specification: formalize the crucial details of the problem that the algorithm is intended to solve
        - it will have to specify how the inputs and outputs of the algorithm are related, though there is no general requirement that the specification is complete or non-ambiguous
2. Does it really do what it is supposed to do?
    - Verification: verifying whether the algorithm is indeed correct
3. How efficiently does it do it?
    - Performance analysis: the efficiency or performance of an algorithm relates to the resources required by it, such as how quick it will run, or how many ram it will use.

## 1.3 Data structures, abstract data types, design patterns
- data structure: denote a particular way of organizing data for particular type of operation
    - abstract data types: defined only by the operations that may be performed on them
        - abstract data type are like user defined data type on which we can perform functions without knowing what is there inside the datatype and how the operations are performed on them
    - primitive data types: used to store the raw data of real world which could be numbers, fractions, text at very basic level
        - e.g. integers or strings

- encapsulation: the implementational details are hidden from the user and protected from outside access

`
even higher level of abstraction
`
- design patterns: describe the design of algorithms, rather the design of data structures
    - they provide a general structure for algorithms, leaving the details to be added as required for particular problems.
    - these can speed up the development of algorithms by providing familiar proven algorithms structures that can be applied straightforwardly to new problems
