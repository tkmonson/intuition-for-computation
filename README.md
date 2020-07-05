# Intuition for Computation
## A Guide for Programmers and Curious Minds

This is an open-source work of non-fiction about computer science and software engineering. It also delves deep into some concepts in philosophy, mathematics, linguistics, and cognitive science. It is a passion project, written mostly for myself, to keep a hard record of my knowledge and to keep track of how topics fit together in my conceptual web. It is an ongoing work-in-progress, and I intend to finish it eventually.

## Motivation

I think the full concept of *Intuition for Computation* is that education should be a narrative experience, that any serious, extended course of study should be told in the form of a carefully crafted story. All of the great ideas and theories of philosophy, mathematics, and science were built on the foundations of previous great ideas and theories, and so much of the why of technical jargon is historical in nature, bits of slang or metaphor, old loanwords from other fields or simply from the culture.

There is a web of academic influence that relates great thinkers to each other throughout time. These were human beings who formed relationships with one another, who wrote letters to one another, who read and cherished and critiqued and built on each other's work; they all experienced great moments of joy and despair, unavoidable hardships, and long periods of intense, active learning before brilliance. And there are narrative threads that can be sewn between these people in this relational web, and threads from seemingly distinct fields can be woven together.

It would be a serious textbook, but all of the formality would be preceded by developed characters, plot, and ideas painted in broad strokes. And gradually the technical vocabulary will be introduced, in context, by tracing etymologies and explaining metaphors, and it will be used precisely and regularly so that the reader begins to consider it all an intuitive part of their everyday language. They develop a personal ontology of these abstract concepts and can read mathematical and logical formulas and code like it is English. They are motivated to continue the hard, constant uphill that is active, technical learning because they are invested in the story, and they want to see how it ends. Imagine how inspirational it would be to have an education where you spent years learning the historical and human side of your field, refining your ideas from top-level philosophical questions to well-defined theories to systems of many models and perspectives, just as the chain of thinkers did all throughout the time before you, and to find at the end that there is no ending, only endless doors. Someone hands you a pen and advises you to keep track of where you are going and where you have been, knowledge-wise.

It would detail computation in all of its forms: as the manual process of writing out calculations to get an answer, as the movement of bits in a computer, as the cognitive act, as the writing of programs, as the building of software, and as the building of society. And beyond that it would trace the frontier: beyond here lies machine learning, and over yonder is quantum computing, and thereabouts is cryptography. And it would end with a request that readers consider the ethics of their work and take responsibility for what they bring into the world.

## The Structure of the Work

There are three main files: `intuition-for-computation.tex` (the "main" source code file), `intuition-for-computation.pdf` (the book itself), and `preamble.sty` (the software packages and custom typesetting commands). The contents of this work are categorized in four administrative groups: the front-matter, the body-matter, the appendices, and the back-matter.

1. The *front-matter* consists of elements that comes before the start of Volume I, which is the formal beginning of the book. This includes the front cover, the inside cover, the table of contents, the epigraph, the preface, the acknowledgements, and the introduction. All of these elements exist outside of the main narrative.

2. The *body-matter* consists of elements that form the body of the text, the main narrative. This is the largest group, and it is further split into five *volumes*, each of which is further split into *chapters*, each of which is further split into *sections*. The structure of `/2-body-matter/` is given below:

* `/2-body-matter/`
    * `volume1/`
        * `c1-cognitive-ontology.tex`
        * `c2-metaphysics-natural-philosophy-and-physics.tex`
        * `c3-information-and-communication.tex`
        * `c4-logic-and-mathematics.tex`
        * `v1-philosophy-of-computation.tex`
    * `volume2/`
        * `c5-automata-theory.tex`
        * `c6-computability-theory.tex`
        * `c7-computational-complexity-theory.tex`
        * `c8-computer-architecture.tex`
        * `v2-theory-of-computation.tex`
    * `volume3/`
        * `c9-type-theory.tex`
        * `cA-algebra-and-category-theory.tex`
        * `cB-abstract-data-types-and-data-structures.tex`
        * `cC-algorithms.tex`
        * `v3-types-structures-and-algorithms.tex`
    * `volume4/`
        * `cD-programming-language-theory.tex`
        * `cE-specification-and-implementation.tex`
        * `cF-operating-systems.tex`
        * `cG-practical-computing.tex`
        * `v4-computer-programming-and-operation.tex`
    * `volume5/`
        * `cH-software-engineering-processes.tex`
        * `cI-design-patterns.tex`
        * `v5-software-craftsmanship.tex`

Note the two different kinds of LaTeX files, `c` and `v` for chapter and volume respectively. The chapter files contain the bulk of the text of this work, and they are divided internally into sections, subsections, and subsubsections. The volume files collect the chapter files and load them in the correct order; they also allow for an introduction and a conclusion to the volume.

Note also that some of these chapters are more developed than others and some of these titles are just placeholders for very large, nebulous areas of interest whose details are being hammered out. Notes for each chapter and volume can be found in the `/notes/` directory, with names like `c1n.md` and `v3nIntro.md` (the `n` suffix stands for "notes"). The notes are written in Markdown for now, but I may convert them to LaTeX later. In the future, there will be one note file for every little topic instead of only one for a whole chapter. The notes are printed into the PDF at the very end.

3. The *appendices* contain all of the supplementary material. This includes material that is interesting but too tangential to include in the main narrative, reflective pieces of writing, and resources like the bibliography and glossary. Notes for each appendix can be found in the `/notes/appendices/` directory.

4. The *back-matter* consists of elements that come after the main narrative and after any supplementary material. Currently, it consists of only the "The End" page, but it may acquire a few more elements.

## The Steps to Completion

0. Gain intuition in the hardest areas, the stuff that I do not understand well enough (e.g. abstract algebra, category theory, programming language theory). Read textbooks, take detailed notes, fully comprehend the subjects.

1. Write a list, in no particular order, of every little topic/concept you want to address (there will probably be hundreds). Make sure each topic/concept is small enough that you can dive deeply into it.

2. Make a file for each, and build a rough file system to impose a small amount of structure on the project.

3. Pick a topic and write about it to your heart's content. Fill the file with facts, definitions, quotes, ideas... just make sure all of it is directly relevant to the topic. Do this for all of the files (this is the part that will take years). If you think that you need to write code libraries for the text, do so.

4. Determine the actual order of topics in the narrative (it does not have to be 1:1 with the file system, things can be split up, combined, and scattered throughout the narrative). Start filling in details, where characters show up, where storylines start and end. How non-linear is the narrative? Do you notice any interesting patterns that inspire you to make an interesting structural choice in the order? The order of topics is arguably one of the most important elements of the work, and clear planning will allow for a smoother writing process.

5. Standardize your typesetting. Find the optimal way to create diagrams, algorithms, code blocks, graphs (elements between text). Structure the project according to the order you determine in Step 4. The code should be clean and creating non-text elements should be fluid and easy.

6. Write the final draft, start to finish. Because you have already largely decided the narrative, you can focus on the poetry of your writing, the words you choose. You can push and pull according to what you know is coming next (or what you know will appear much later).

7. At this point, the main text is written and typeset. Now, you can focus on aesthetics. Standardize anything you've made already, draw digital art, make nice title pages, put that extra sprinkle of craftsmanship on it. Also, make sure the appendices are written, the bibliography is handled, the introduction and preface are written, the licensing is handled, all the little things.

8. Time for peer review. Give it to friends and family, get their thoughts. Make edits.

9. Publish. Advertise. Read it yourself. Determine if you want to add anything in a future version. Think about what to do next with your life.

## Contact

tkmonson@protonmail.com
