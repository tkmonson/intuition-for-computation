# Notes for Chapter 6: Computability Theory

Cybernetics

Algorithm characterizations (wiki)

Godel says that Turing's analysis of computability is perfect (Interpreting Godel: Critical Essays, p. 118, cited in Wiki: Logic in computer science)

Decision problems

## The Scope of Problem Solving

Rewrite -- what are problems, why are they worth solving, what is calculation, what is computation?

Domains of discourse / universes in classical logic are just types in type theory. Top = true in every universe, Bottom = true in no universes (false)

Use sequent notation to explain axioms
Formal systems
Proof calculi (Hilbert)
Automata are formal systems

Curry-Howard: proofs and programs are the same thing. 

A deductive system is a "calculus"
Argument - set of statements (premises) and a conclusion in a language
Premises can be axioms or theorems
Logical consequence
Truth-bearer
Deductive reasoning is applied to an argument to create a deduction (argument + steps of reasoning)
Composing a deduction is a way to prove validity
Composing an induction is a way to assess strength
Venn diagrams
Reasoning is a set of rules of inference
Inductive/deductive "steps"
Proof - deduction from "known truths" (axioms and proven theorems), proves soundness
Data validation proves cogency?
Argument vs explanation
Validity/soundness

### Informal Logic

Discuss the logical reasonings comparatively. 3 paths in life. Certain vs uncertain. Binary vs multi-valued.

Interlocuters
Fallacious reasoning
Formal vs informal (indep of interpretation)

### Formal Logic

Common logical symbols wiki
Domain of discourse / universe
Deduction is impossible in non-axiomatic systems because we don't know what the axioms of the Universe are.

What is logic?

What is early logic?

Syllogistic logic (categorical reasoning, motivated by science 13:45)
Stoic logic

Informal logic is not always explicit. It may have implicit elements that must be made explicit by analysis.
Formal logic, traditionally symbolic logic, now called mathematical logic

What is modern logic? ("Arguments and the forms they make take")

Hobbes - thought as computation
Boolean logic
Frege, logicism
Class - Russell's paradox

Logical and non-logical symbols
Categorematic and syncategorematic terms (individual meaning)
Formal systems
Reason vs. logic -> Humans vs. computers
Model theory

Set theory is intertwined with two-valued logic via the membership function

Fuzzy set theory
Membership functions between 0 and 1

## The Ballad of Georg Cantor

Introduce the problem of the "size" of infinity.
Example of the unit circle. The unit circle has a circumference of 2pi. It has circumference values of [0,2pi] in mathbb{R}. Another way of saying this is that it has \textit{central angle} values of [0,2pi] in mathbb{R}. The difference between that and, say, a\_n=frac{1}{4}\*n, n=[0,7] in mathbb{Z} is that all real intervals have an infinite number of possible values. But what happens when you go past 2pi, \textit{beyond infinity}. You expand the infinite interval\dots to a another infinite interval. You'd be hard-pressed to find someone who argues that the interval [0,4pi] is \textit{not} bigger than [0,2pi]. And yet, the intervals have the same "density" (they both have an infinite number of values). So the space doubled, and the density remained the same. This is not familiar to us. "Size" (number of elements) is not a useful measure of infinite sets. We need to generalize to cardinality.
Are there infinite sets of different cardinalities? What if you doubled your interval an infinite amount of times?

Trying to work directly with absolute infinity is trouble. Singularities.

### Computable Functions and Computable Numbers

Definitely discuss Principia Mathematica, it's very important step in formalizing mathematics, and Godel proves its goal to be ultimately impossible.
The vicious circle principle

## Hilbert's Program and Godel's Refutation of It

### Hilbert's Second Problem

Two blue boxes: philosophy of mathematics and Hilbert creating the field of metamathematics with his 1900 speech
Influence of Plato and Euclid on philosophy of mathematics
Mathematical realism, mathematical Platonism
The Big 3 during the crisis: logicism, intuitionism/constructivism, formalism

Before we discuss G\"odel's landmark theorems in mathematical logic, we must understand a bit about the theory that they describe. G\"odel's theorems on the \textit{completeness}, \textit{soundness}, and \textit{incompleteness} of logical theories are foundational to a discipline in mathematical logic known as \textit{model theory}. \\

Maybe edit above paragraph as you learn more

Most mathematical disciplines focus on a particular mathematical object or structure. An \textit{object} in mathematics is anything that can be formally defined using logic (typically, first-order logic). Given a set-theoretic foundation for mathematics, every mathematical object can be defined as a \textit{set}. A set is a collection of well-defined, distinct objects, and it is itself also an object. Sets can represent objects such as \textit{numbers}, \textit{matrices}, \textit{functions}, \textit{relations}, \textit{points}, \textit{polygons}

### Godel's Incompleteness Theorems

If it's true, it's provable.

Modern proof theory treats proofs as inductively defined data structures. There is no longer an assumption that axioms are "true" in any sense; this allows for parallel mathematical theories built on alternate sets of axioms

Verifying a set is recursive by checking that each member can be formed from the axioms (inductively defined)

Recursion vs counting

Godel's thoughts on logical intuition

### The Halting Problem

Peano, ZFC

Hilbert's program
ent-shy-dungs-probe-leem
Entscheidungsproblem, which asked whether there was a mechanical procedure for separating mathematical truths from mathematical falsehoods

Church-Turing thesis

Partial recursive functions

Lamda calculus

Turing machines
The halting problem
Something is recursively enumerable when its elements can be counted using recursion. Recursion is a more natural counting method than iteration for sets because sets have no order.

MapReduce is a monoid based alg

BB: Computability is Recursion
    A function can be written iteratively and recursively
    Tail recursion - iterating via recursion
    Some tasks are suited to iteration, others to recursion. What is the deciding factor?
    Recursively enumerable / recursive => computable
    In a well-behaved recursive function, you approach a base case => there is an end in sight for the computation.

## Turing Degrees

Posits, chains, antichains
Turing degrees are a join-semilattice
r.e. degrees are dense
Turing degrees of language
Post problem

