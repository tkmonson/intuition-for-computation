# Notes on "Aristotle's *Prior Analytics* and Boole's *Laws of Thought*" (Corcoran 2003)

Thesis: Aristotle is the founder of logic as *formal epistemology*. Boole is the founder of logic as *formal ontology*.

## 1. Introduction

Aristotle's logic has three parts:

1. a limited domain of propositions expressed in a formal, canonical notation
2. a method of deduction for establishing validity of arguments with an arbitrary number of premises
3. a method of countermodels for establishing invalidity

Boole's logic has the first part, but his methods of derivation are neither sound nor complete.

Boole accepted Aristotle's logic and wished to expand on it. He did not find fault with what Aristotle produced, but with what he did not produce.

*Prior Analytics* marks the start of logic. *Laws of Thought* marks the start of mathematical logic. But logical deduction has been traced back to Thales. The study of logic began as a way of identifying what is proof and what is persuasion.

## 2. Colloquial and formalized languages

1. The grammatical-logical discrepancy: sentences vs. propositions.
2. The grammatical form does not necessarily correspond to the logical form.

Sentence: a series of interrelated words.
Proposition: a series of interconnected meanings or concepts that may or may not have been expressed in words.

Two sentences may differ but express the same proposition. Often, however, one will more closely correspond to the logical form.

Elliptical sentences are shortened for convenience. Expletive sentences are lengthened for emphasis. Both diverge from the logical form of the proposition.

Russell's theory of descriptions: there is a large class of sentences that, contrary to their appearances, express existential proposition.

Single quotes are used to denote sentences and other expressions such as words, phrases, and symbols. Double quotes are used to denote propositions and other meanings. For example, 'square' is a six-letter English word, and "square" is a concept.

A "system of logical paraphrase" is required to translate natural language sentences into sentences that correspond to the logical form of a proposition. Then, a set of transformations is created in order to implement logical inferences. From a set of premise-sentences, one can then use this newly created *logical calculus* to find all consequent conclusions.

The ultimate goal in designing a logical notation is to create a language in which each sentence expresses exactly one proposition and in which there is no grammatical-logical discrepency. The semantic structure will remain the same regardless of any changes in syntax. Thus, there is really only one *logically perfect language* or *formalized language* for any given domain.

Boole agree with Aristotle that every simple proposition is composed of three constituents: the *subject*, the *predicate*, and the *connector* (or *copula*). In the proposition "Every square is a rectangle," the subject is "square," the predicate is "rectangle," and the connector is "Every ... is a \_\_\_." Aristole would rewrite this sentence as "Rectangle belongs-to-every square," which has the pattern P-c-S (Predicate-connector-Subject). (The subject and predicate are called "terms" because they are the "terminals" or ends of the rewritten sentence.)

Aristotle had four connectors in his logic, according to which he classified propositions:

1. Universal affirmative: "belongs-to-every"
2. Universal negative: "belongs-to-no"
3. Existential affirmative: "belongs-to-some"
4. Existential negative: "does-not-belong-to-every" or "non-belongs-to-some"

Contrary to Boole's belief, the subject-connector-predicate view does not characterize every proposition. For example, it cannot not express co-extensionality propositions.

Aristotle was very interested in taxonomy and the species-genus relationship. This may have influenced the design of his logic to have three constituents rather than the two obvious substantive ones (subject and predicate). His focus on relations such as *inclusion* and *exclusion* allowed him to recognize the copula as a distinct constituent.

Boole agrees that the subject and predicate should be substantive (i.e. they should be nouns or noun phrases). 'Snow is white' is thus translated to the logical paraphrase 'Snow is a white thing.'

Aristotle did not say anything about complex terms, so it is assumed that he regarded terms as necessarily unitary. Thus, he would not have been able to deduce "Every male human is mortal" from "Every human is mortal" with his logic because "male human" would be interpreted as a unitary term "male-human" which has no relation to the term "human."

## 3. Boole's view of his relation to Aristotle

Boole's goals in *Laws of Thought*:

1. To ground Aristotle's logic in mathematics rather than in philosophy.
2. To broaden Aristotle's logic in order to represent a wider domain of propositions and incorporate inferential transformations from mathematics.

# 4. Boole's reconstruction of Aristotle's logic

Boole tries to show how the four connectors can be reduced to one. For Boole, "Every square is a polygon" or, as Aristotle would put it, "Polygon belongs-to-every square" is really an *equation* and is better written as "Every-square [is-one-and-the-same-as] a-polygon" or "All-squares [is-one-and-the-same-as] some-polygons." Thus, Boole argues that quantifiers should be considered parts of the subject and predicate, not of the connector. His form is then S-is-P or S=P.

1. Propositions are equations between class-terms, not substantive predications.
2. Quantified-subject and quantified-predicate expressions are used as class-names.

Statement 2 is problematic. What class does "some polygons" correspond to? It is ambiguous, and thus not perfectly logical. Is 'all squares' the name for the class of squares? No, it is a plural noun, whereas the class of squares is a singular entity.

For Boole, the only connector is =, which represents equality in the sense of *numerical identity*. The connector is called the *is-of-identity*. For example, "Mark Twain is Samuel Clemens" means that "Mark Twain" and "Samuel Clemens" are the exact same thing. However, in "Mark Twain is clever," "is" is an *is-of-predication*.

With only one connector, propositions cannot be classified by connector type. Boole argues that quantifiers and words like 'universal,' 'particular,' 'affirmative,' and 'negative' should be applied to terms, not to propositions.

1. Universal affirmative: "all squares"
2. Universal negative: "all things not squares"
3. Particular affirmative: "some squares"
4. Particular negative: "some things not squares"

Unlike Aristole, whose terms are always logically unitary, Boole wishes to treat as logically complex those terms which are expressed by grammatically complex expressions. He handles these complex terms with mathematical operators: x ('and'), + ('or'), - ('not').

Aristotle did not recognize the universal term 'entity' or 'thing' nor did he recognize the null term 'nonentity' or 'nothing.' Subjects and predicates are typically represented by non-logical symbol, but things like the universe of discourse or the null class would likely be considered Tarskian logical notions and would need to be represented by logical symbols. Thus, the logical form of a proposition including a 'thing' or 'nothing' would be atypical. Boole, on the other hand, includes 'thing' and 'nothing' in his logic as logical terms.

In his earlier work, Boole used the symbol '1' to refer to "the universe," the most comprehensive class. In this case, '1' is a *label-word*, a word whose referent is fixed. In contrast, a *pointer-word* or *indexical* is a word whose referent depends on context (e.g. 'you' or 'here'). In *Laws of Thought*, Boole instead uses '1' to mean "the universe of discourse," whose extension depends on context. In doing this, Boole allows the same language to be used in many different interpretations.

In each modern mathematical theory, the special universe of discourse contains all of the entities that are subjects of the propositions of the theory. For example, the universe of discourse for group theory contains groups; groups are the entities that are described in group theory.

For Boole, not only was each propostion about some entity or entities in the universe of discourse, but it was also about the universe of discourse itself. Moreover, both of the terms of an equation contained the concept of the universe of discourse and, indeed, each expression of a term of an equation contains at least one occurrence of the character '1' referring to the universe of discourse.

This is based on the principle that the mental process of formulating a proposition begins with conceiving of the universe of discourse. So if 'x' occurs by itself, it is elliptical for the class-name 'x(1)' (e.g. the meaning of 'human' has a logical form corresponding to 'entity that is a human').

## 5. Systems of deduction

Because Boole's propositions are equational, his logic is capable of making the same equational inferences made in mathematical analysis in addition to the syllogistic inferences of Aristole's logic.

Aristotle's system of deduction is based on epistemically immediate (e.g obvious, trivial, or fundamental) inferences (conversion, obversion, contraposition). In Boole's system, these inferences are not considered immediate.

Boole believed that he had found the sought-after *logically perfect language*.

Aristotle took his deductive system to be an object of scientific interest. He proved that every conclusion from a given set of premises using any or all of his rules of inference is also deducible from the same premise set without the use of the Darii and Ferio rules. Thus, two of the rules in his system are eliminable. Boole did not study his own system in this way, perhaps because he was not interested in finding a complete system.

Neither Aristotle nor Boole limited the number of premises given or the number of intermediate conclusions required for a deduction. But Aristotle rejected the possibility of an infinite premise set.

Aristotle's formal language had no tautologies, so he did not recognize the possibility of a zero-premise deduction (i.e. a logical axiom). Boole did recognize the role that tautologies play in the deduction of non-tautologies, but he did not notice the existence of zero-premise arguments.

Aristotle's two-premise eliminability result is considered proof-theoretic (or, if that term sounds too absolutist, deduction- or derivation-theoretic). In studying the structure of his own logic, Aristotle raised metalogical questions, such as that concerning deductive completeness (i.e. whether every consequence of the given propositions is deducible from them within the logic).

## 6. Laws of thought

Boole expresses laws of non-contradiction as "0=(s*(1-s))," stating that it is a law of logic or a "law of thought" rather than a law of metaphysics. Aristotle's logic does not have support for such laws, but Aristotle did recognize a single law of non-contradiction that applied to all qualities: "a subject cannot both have and not have the same quality."

Because Boole has no variables and no way to universally quantify an equation, he can only express instances of his laws of thought, not class-wide statements. For example, he cannot state formally that "for every class X, 0=X(1-X)," even though he can list every instance of this statement.

Formal ontology establishes general laws that govern the concepts common to all sciences. Before Boole, logic was just formal epistemology, the study of formal validity and invalidity. Frege and the logicists focused on the ontological ideas raised by Boole.

Laws of commutativity have the logical form "(e*a)=(a*e)" (e.g. "being an equilateral and an equiangular is being an equiangular and an equilateral"). Boole also discovered *index laws*, which have the logical form "(a*a)=a" (e.g. "being both a circle and a circle is being a circle").

Boole's logic could express infinitely many laws of thought, each having different logical forms. Aristotle's logic could not express even one law of thought. It was unable to express tautologies like "Every square is a square." Aristotle simply assumed that predication involved one thing being predicated by *something else*.

## 7. Boole's inadequacies

Boole's projects: the algebra of classes, analyzing the logic of the English language, truth-functional logic, reconstructing syllogistic logic, epistemology of logic, logic as formal ontology.

Flaw #1: Boole overlooked indirect reasoning (reductio ad absurdum), one of the most common and productive forms of inference. In Aristotle's logic, given a premise set and a conclusion, one could prove the conclusion by deriving a contradiction from the premise set and the negation of the conclusion.

Flaw #2: The Solutions Fallacy. A solution to an equation is not necessarily logically deducible or implied by the equation. 'x=(x*y)' does not imply the solution 'x=0' or 'y=0' ('x=1' and 'y=1' would also work). However, 'x=0' *does* imply 'x=(x*y).' Boole thought that one could replace equations that express universal propositions with their solutions.

Boole compares syllogistic reasoning to equation-solving. Thus, he thinks of conversion as equation-solving, not as a form of inference. This may be why he neglect to consider indirect reasoning because there is no indirect equation-solving.

Boole's logic has no way to deny an equation (e.g. inequality, "it-is-not-the-case-that"). While it does have the NOT operator, that is not the same thing. It is more logical to avoid all negative expressions except 'it is not the case that' and to always use parentheses with that expression. Aristotle did not use this negation either, but he could still express denial by considering the reductio assumption of a proposition, its contradictory opposite.

Boole may have been blinded to the solutions fallacy in part because of his use of the letters 'x,' 'y,' and 'z' for both propositional terms (instead of 'a,' 'b,' and 'c') and metalanguage variables (instead of 'S,' 'M,' and 'P') when they should be reserved for *unknowns*. This notation makes it seem like you are supposed to solve for those terms, which is not the case.

Once Boole's fallacious intermediate conclusions are deleted, there is no cogent way to fill the resulting gaps in the deduction. The ultimate conclusions cannot be reached with his logic. Additionally, Boole did not deduce the equational analogues of some of Aristotle's immediate inferences and thus did not reduce syllogistic logic to equational logic.

Boole's three signs of operations do not denote what are known today as Boolean operations. He did not present a decision procedure, and he did not devise 'Boolean algebra.'

Some dislike Boole's logical definitions of plus and minus. If the classes indicated by 'x' and 'y' share no elements, then '(x+y)' refers to their union; if they do share elements, '(x+y)' has no referent and is undefined. Similarly, 'x-y' is only defined if the class indicated by 'x' contains all of the elements of the class indicated by 'y.'

Boole is criticized for his lack of relational logic (less than, greater than). He did not discover much equational logic either, considering that he does not even consider the law of associativity. He was more interested in the algebra of logic than in the logic of algebra.

## 8. Conclusion

Aristotle is the founder of logic, but his work is built on the deductive reasoning in geometry that was practiced by Plato's Academy and on the ideas of proof and fallacy that were brought up by Socrates. Boole is often called the founder of mathematical logic.

The method of countermodels for independence proofs (that demonstrate the absence of logical consequence), a cornerstone of model theory, is covered by Aristotle but not by Boole. The device of reinterpreting language, found in the modern form of the method of countermodels, is present in *Laws of Thought* but not in *Prior Analytics*.

The device of reinterpreting non-logical constants is not yet present in Tarski's 1936 'On the concept of logical consequence,' one of the defining papers of model theory. Instead, Tarski replaces non-logical constants with variables.

Boole has a place in the history of proof theory. His idea of reinterpreting a formal language opened the way for thinking of a language without any interpretation, and this is one of the basic ideas of proof theory.

Neither Aristotle nor Boole had variables in their formalized object languages. Frege had quantified variables in his concept script.

Aristotle laid down the groundwork for a science of determining validity and invalidity of arguments. Boole laid down the groundwork for a science of formal laws of being. Boole's greatest achievement was convincing the world's logicians that logic should be pursued mathematically.
