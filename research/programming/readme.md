# [**programming**](https://my.mindnode.com/nyxpNazrso6eyV3M4RNGS9sUyXfNzTXq6pGhRYLZ#-1120.9,46.4,-1)

- is a process that leads from an original formulation of a computing problem to an executable computer programs


## [bitwise operations](https://my.mindnode.com/jjdFxBtm7BCMmZBfFHwwyRh3q3awMFxbXePMs4Cy)

- operate on one or more bit patterns or binary numerals at the level of individual bits  
- it is a fast, simple action directly supported by the processor, and is used to manipulate values for comparisons and calculations  
- the operators are :  
	- AND  
	- OR  
	- NOT  
	- XOR (Exclusive Or)  
	- NAND (Not And)

## [design patterns](https://my.mindnode.com/FPsEgZQpPDCmzQSspyY2AKqGNTsLGrAKpg6sXk12#1041.1,-95.8,0)

- are general reusable solutions to a commonly occurring problem within a given context in software design  
- it is not a finished design that can be transformed directly into source or machine code  
	- it is a description or template for how to solve a problem that can be used in many different situations

## [dynamic programming](https://my.mindnode.com/cpxi9EqMbbF7cvq3vqD4pDQLwHetX81qagPEXi99)

- is a method for solving a complex problem by breaking it down into a collection of simpler subproblems, solving each of those subproblems just once, and storing their solutions - ideally, using a memory-based data structure  
	- next time the same subproblem occurs, instead of recomputing its solution, one simply looks up the previously computed solution, thereby saving computation time at the expense of a (hopefully) modest expenditure in storage space  
- the technique of storing solutions to subproblems instead of recomputing them is called ‘memoization’  
- dynamic problem algorithms are often used for optimisation  
  
method of solving problems, using this method, a complex problem is split into simpler problems, which are then solved, at the end, the solutions of the simpler problems are used to find the solution of the original complex problem

## [paradigms](https://my.mindnode.com/qqjRxmiDoMyKteYicvarwjrgMgpsYJjLWgXsD5Wn#767.7,-730.8,2)

- are a way to classify programming languages according to the style of computer programming   
- features of various programming languages determine which programming paradigms they belong to  
	- as a result, some languages fall into only one paradigm, while others fall into multiple paradigms  
- common paradigms include  
	- imperative which allows side effects  
	- functional which disallows side effects  
	- declarative which does not state the order in which the operations execute  
	- object-oriented which groups code together with the state the code modifies  
	- procedural which groups code into functions  
	- logic which has a particular style of execution model coupled to a particular style of syntax and grammar  
	- symbolic programming which has a particular style of syntax and grammar

### declarative

- is a style of building the structure and elements of computer programs that expresses the logic of a computation without describing the control flow

- [functional ✨](https://my.mindnode.com/yLFW2vMCgshzaepsYcYDCpYnRBFktycVYmjtRwcF)
  - is a style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data  
  - in functional code, the output value of a function depends only on the argument that are passed to the function, so calling a function f twice with the same value for an argument x will produce the same result f(x) each time  
  - eliminating side effects (changes in state that do not depend on the function inputs), can make it much easier to understand and predict the behaviour of a program  
  - lambda calculus provides a theoretical framework for describing functions and their evaluation

- logic
  - is largely based on formal logic  
  - any program written in a logic programming language is a set of sentences in logical form, expressing facts and rules about some problem domain

- dataflow
  - models a program as a directed graph of the data flowing between operations, thus implementing data flow principles and architecture

- constraint
  - is a paradigm wherein relations between variables are stated in the form of constraints  
  - constraints differ from the common primitives of imperative programming languages in that they do not specify a step or sequence of steps to execute, but rather the properties of a solution to be found  
  - constrain programming can be expresses in the form of constrain logic programming, which embeds constrains into a logic program

### imperative

- uses statements that change a program’s state  
- imperative program consists of commands for the computer to perform  
	- it focuses on describing how a program operates

- [object oriented](https://my.mindnode.com/bXt6DgouTpBrCURxSzAyvZxMEsSU4pd4ecBVtRzn)
  - is based on the concepts of ‘objects’, which may contain data, in the form of fields, often known as attributes; and code, in the form of procedures, often known as methods  
  - a feature of objects is that an object’s procedures can access and often modify the data fields of the object with which they are associated (objects have a notion of ‘this’ or ‘self’)  
  - in OOP, computer programs are designed by making them out of objects that interact with one another  
  - most popular object oriented languages are class-based, meaning that objects are instances of classes, which typically also determine their type

- procedural
  - is derived from structured programming, based upon the concept of the procedure call  
  - procedures, also known as routines, subroutines, or functions, simply contain a series of computation steps to be carried out  
  - any given procedure might be called at any point during a program’s execution, including by other procedures or itself

### metaprogramming

- is a programming technique in which computer programs have the ability to treat programs as their data  
- it means that a program can be designed to read, generate, analyse or transform other programs, and even modify itself while running  
- it can be used to move computations from run-time to compile-time, to generate code using compile time computations, and to enable self-modifying code

- [template metaprogramming](https://my.mindnode.com/GkpWKLpuRFrkF6zPEW92CzDtyaxua4s7YyAmZ4Kn)
  - is a metaprogramming technique in which templates are used by a compiler to generate temporary source code,, which is merged by the compiler to generate temporary source code, which is merged by the compiler with the rest of the source code and then compiled  
  - the output of these templates include compile-time constants, data structures and complete functions  
  	- the use of templates can be thought of as compile-time execution

## [testing](https://my.mindnode.com/1qGKADJWJ2MtkLpVgCUF5Pooa4iVKbHjTfKfYGNu)

- software testing is an investigation conducted to provide stakeholders with information about the quality of the product or service under test  
- it involves the execution of a software component or system component to evaluate one or more properties of interest  
	- it indicates the extent to which the component or system under test  
		- meets the requirements that guided its design and development  
		- responds correctly to all kinds of inputs  
		- performs its functions within an acceptable time  
		- is sufficiently usable  
		- can be installed and run in its intended environments  
		- achieves the general result its stakeholders desire

### [test driven development](https://my.mindnode.com/ey6QYxyUo6JqQ6tDmmRRLykwjpr7ybbEf5fcicZr)

- is a software development process that relies on the repetition of a very short development cycle  
	- requirements are turned into very specific test cases, then the software is improved to pass the new tests, only  
- it encourages simple designs and inspires confidence   
- a typical test driven cycle is  
	1. add a test  
	2. run all tests and see if the new test fails  
	3. write the code  
	4. run tests  
	5. refactor code

### [unit testing](https://my.mindnode.com/z3wLxo6zw1KEpPs1kryj51ToaDH3RkfEDQx4GRDR)

- is a software testing method where units of source code, sets of one or more computer program modules together with associated control data, usage procedures, and operating procedures, are tested to determine whether they are fit for use  
- one can view a unit as the smallest testable part of an application  
- ideally, each test case is independent from the others

## [exception handling ✨](https://my.mindnode.com/xEiGQnjcJeqyxvxpxspGJR7q4zDQPawRYMpJDqVj)

- exception handing is the process of responding to the occurrence, during computation, of exceptions (anomalous or exceptional conditions requiring special processing - often changing the normal flow of program execution)  
- in general, an exception breaks the normal flow of execution and executes a pre-registered exception handler

## [abstraction](https://my.mindnode.com/7aNxJDAnKfSqGHhHpnpewSeDdFMmCY5tj32fdFqH)

- is a technique for arranging complexity of computer systems  
- it works by establishing a level of complexity on which a person interacts with the system, surpassing the more complex details below the current level  
- the programmer works with an idealised interface (usually well defined) and can add additional levels of functionality that would otherwise be too complex to handle  
- abstraction can apply to control or to data  
	- control abstraction is the abstraction of actions while data abstractions is that of data structures  
	- control abstraction involves the use of subroutines and control flow abstractions  
	- data abstraction allows handling pieces of data in meaningful ways  
- the notion of an object in object-oriented programming can be viewed as a way to combine abstractions of data and code

## [software verification](https://my.mindnode.com/i2Tmz28SzbT3WCq6aqrQy75sy226sNxAkZ3aABxG)

- is a discipline of software engineering whose goal is to issue that software fully satisfies all the expected requirements  
- there are two fundamental approaches to verification   
	- dynamic verification, also known as Test or Experimentation (this is good for finding bugs)  
	- static verification, also known as Analysis (is useful for proving correctness of a program although it may result in false positives)

## [dependency injection](https://my.mindnode.com/L1ZfeUJUTiLaJG9RUbE47q6QkDkYUxBGMA9URp2E)

- is a technique whereby one object supplies the dependencies of another object  
- a dependency is an object that can be used (a service)  
- an injection is the passing of a dependency to a dependent object (a client) that would use it  
	- the service is made part of the client’s state  
	- passing the service to the client, rather than allowing a client to build or find the service, is the fundamental requirement of the pattern  
- the intent behind it, is to decouple objects to the extent that no client code has to be changed simply because an object it depends on needs to be changed to a different one

## [syntax trees](https://my.mindnode.com/55ZLtTbzDZJV6aXqXUxN92g6Ps7GMbnsEpjD7sqq)

- are tree representations of the abstract syntactic structure of source code written in a programming language  
- each node of the tree denotes a construct occurring in the source code  
- they are used in program analysis and program transformation systems  
- they are data structures widely used in compilers due to their property of representing the structure of program code  
	- an AST is usually the result of the syntax analysis phase of a compiler  
	- it often serves as an intermediate representation of the program through several stages that the compiler requires, and has a strong impact on the final output of the compiler

## [static analysis](https://my.mindnode.com/3sCkLyCxbePrDHzrCRpVEQX6xfMHFPSrN6tRzMfx)

- is the analysis of computer software that is performed without actually executing programs (analysis performed on executing programs is known as dynamic analysis)  
	- in most cases the analysis is performed on some version of the source code, and in the other cases, some form of the object code

## [linters](https://my.mindnode.com/6KxuVfowmW81Teuawc2FedkqG5QxiHwseUg3GZDP)

- linting is the process of running a   
program that will analyse code for potential errors

## [evaluation](https://my.mindnode.com/NDkKMcxWGi5vHMwEbFzpM3yof8orjxvCyPuGUvCn)

- is a systematic method for collecting, analysing and using information to answer questions about projects, policies and programs, particularly about their effectiveness and efficiency 

## [memory](https://my.mindnode.com/wbRrdVuWerWQMHiPNrW7KdeLc9WFyz2EzBBQSgSd)

- how to effectively manage data whilst programming

## [type system ✨](https://my.mindnode.com/S5yqn46mnWuPPzHzQN5yaZPzoJ2gCfTbJWzJt4qZ)

- is a set of rules that assign a property called a type to various contracts a computer program consists of, such as variables, expressions, functions or modules  
- the main purpose of it is to reduce possibilities for bugs in computer programs by defining interfaces between different parts of a computer program, and then checking that the parts have been connected in a consistent way  
	- this checking can happen   
		- statically (at compile time)  
		- dynamically (at run time)  
		- or as a combination of static and dynamic checking  
- other purposes of a type system include enabling certain compiler optimisations, allowing for multiple dispatch, providing a form of documentation, etc.  
- it associates a type with each computed value and, by examining the flow of these values, attempts to ensure or prove that no type errors can occur

## [competitive ✨](https://my.mindnode.com/HjzAcCjnzpEcL69NSNYigoEyVeDTUiXLsEh3nM6P)

- is a mind sport usually held over internet or a local network which involves participants trying to program according to provided specifications  
- the competition generally involves a set of logical or mathematical problems and contestants are required to write computer programs capable of solving each problem

## debugging

## [language design](https://my.mindnode.com/SFyx1AMA4eKBbkwq59ymrQz3AEKQMiw8A8SV1WeX)

