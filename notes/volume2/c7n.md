# Notes on Chapter 7: Computational Complexity Theory

Algorithmic information theory, Kolmogorov complexity

Avi Wigderson (2010) proposes mathematical knowability should be based on computational complexity.

## Complexity Classes

Time and space complexity are two different kinds of \textit{computational complexity}. Computational complexity measures how much of a given resource an algorithm requires to run. Time and space just happen to be the resources we are most interested in. That said, computational complexity of \textit{any} kind is an algorithmic concept. Data structures themselves do not have time or space complexity. The algorithms that implement their operations do. However, one could informally say that a data structure "has" a certain space complexity $S$. That is, if a data structure needs to keep track of $n$ values, one could say it must store $S$ elements (assuming all of its operations are implemented optimally). \\

Some complexities you will encounter in this guide will have multiple terms (e.g. $O(m+n)$). Note that if $O(m)=O(n)$, $O(m+n)$ could simplify to either $O(m)$ or $O(n)$. However, if $m$ belongs to a higher order of algorithms than $n$, $O(m+n)$ would simplify to $O(m)$ (the higher bound). \\

