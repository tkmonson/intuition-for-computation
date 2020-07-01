# Notes for Chapter 9: Type Theory

Intentionality and extensionality - types are intensional, classes can be either (wiki - Class (philosophy))
In this case, class is equivalent to the idea of a set in mathematics. Sets can also be defined extensionally and intensionally.
In mathematics, the word class has different definitions based on which foundation of mathematics you are working in. Informally, in mathematics, a class is a collection of mathematical objects. In Zermelo-Fraenkel set theory, a class is informally a collection of sets (which are formally defined, axiomatized). In Von Neumann-Bernays-Godel set theory, the word class refers to the abstract idea of a proper class, which is formally defined. In ZFC, sets are elements of other sets, but classes are not elements of any other class (e.g. the class of ordinal numbers is not a set). In ZFC, sets are objects in your universe, classes are not. Sets are semantic objects, classes are syntactic objects.
Before the foundational crisis of mathematics, the word set was used as an informal term for a collection of things. Set theory formalizes the definition of a set. Cantor's and Russell's paradox revealed that not all collections are sets. A class is any object that can be described in the langauge of set theory. Not all classes are sets. The axioms of set theory apply only to the sets.
A category in category theory is a pair of classes (basically). In this case, the word class means either set or proper class. If both of its classes are actually just sets, the category is \textit{small}. Otherwise, it is \textit{large}.

Essence - philosophy
Curry-Howard Isomorphism
Not all data structures implement abstract data types.

Imperative vs functional ADTs

Talk about how relations are sets (objects)
Functions are deterministic relations

In compsci, Method (can be abstract) vs effective method (steps fully described and finite, can be written in pseudocode) vs algorithm (steps fully described and finite, can be written in pseudocode, calculates the values of a function) vs an implementation of that algorithm. Church-Turing theorem, computability theory and what not... Talk about how every iterative function can be written recursively and vice versa. Any time you use recursion, you're basically adding a stack to the algorithm.

Contiguous or non-contiguous? Array or node?
Mention other ADTs that a DS could implement
Address lack of pictures. Add pictures for ADTs?
Delete operation should acutally be remove. Discuss the distinction.

## The Curry-Howard-Lambek Isomorphism

Recursive composite type = a dynamic data structure

Curry-Howard Isomorphism

Logic programming

Monoids, groups, algebras, coalgebras, etc.
Signatures

F-Coalgebra
Semiautomata and transition systems
Algebraic specification

