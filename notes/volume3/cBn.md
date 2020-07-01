# Notes for Chapter 11: Abstract Data Types and Data Structures

ADTs are "types" of metaphysical objects.
These are just patterns that appear in life. Trees tend to be more common in nature, lists are how humans tend to organize things.
Do "plain old data structures" first: arrays, structs, records, unions, objects
Data type + data structure wiki

What is a module? What is a dictionary?

The subsections should be ADTs. The subsubsections should be data structures. If you really want to discuss a specialized implementation, you can make it paragraph or a blue box. But you should seriously consider pushing the implementations into an appendix for better thematic cohesion.

What do I mean when I say... type (or data type), structure (or data structure), object, instance, class (of objects), implementation
If an element has type $X$, it belongs to a class $X$. We typically speak in terms of types in theoretical computer science (harkening back to Alonzo Church) and in terms of classes in object-oriented programming (harkening back to the programming language Simula, whose designers Ole-Johan Dahl and Kristen Nygaard were harkening back to the idea of a class in philosophy and mathematics).

Iterators

## Lists

Talk about tuples, how they are different than lists, and why the preferred term is list (streams, countable infinity)

### Arrays

Talk about how strings are often implemented with arrays.

### Linked Lists

An interesting example - The Undo & Redo text editing process is a linked list.

## Graphs

Flow networks
Graph coloring
Minimum spanning trees

## Trees

Talk about a "single branch tree" or a "path." Kind of like a linked list, right? Basically, there are two design philosophies to data structures: contiguous and non-contiguous (or node-based).
Discuss the array implementation of a binary tree.
Talk about how file systems are trees
Talk about how this guide is tree-structured (3->3.1->3.1.1)

