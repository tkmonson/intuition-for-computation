# Notes for Chapter 3: Information and Communication

Semiotics
Signal processing (analog and digital)
Language
Coding theory

Thinking information-theoretically / computational philosophy

## Signals and Systems

Signals are messages composed of time-amplitude data

BB: The Rationale for Binary Numbers
    Implementation details: signals, logic levels, noise, power, reliability
    Close relationship with classical, two-valued logic
    Analog computers have many problems: noise, reproducability
    Ternary electronic computers and their issues
    Binary computers and boolean algebra (logic)
    Beyond binary - fuzzy logic (briefly, discuss more deeply later)

Encoding doesn't have to use numerals. It can use letters, pictures, whatever. You can encode anything anywhere.

Information signals
Information systems

All information is encoded and decoded (digital and sensory)

So, we can represent physical things we experience with digital data. If we collect enough data on the properties of these things, we can simulate reality. We can also simulate abstract mathematical phenomena and other abstract things like language and logic. Much of software design is the simulation of mathematical objects.

Structured manipulation = algorithm
The Shannon-Weaver Model of Communication
Sensory, conversation, and machine examples

We need to communicate an algorithm in a language
What kind of language?
First, let's talk about language in general

Serialization or marshalling - translating an object (abstract or concrete) into a format that can be stored, communicated, and deserialized into an object again (terms are not quite synonymous in Java)

Computation with analog data means you are using actual, original, non-replicable quantites. Computation with digital data means you are using simulated quantities that are replicas or model of what you actually care about. We model EVERYTHING with numbers: physics, language, logic, images, video, music.

Pros and cons of digital and analog computation

One can think of digital encoding as a special case of analog encoding, in which a quantity is considered analogous to a sequence of digits that represents a \textit{number}. Because numbers are abstract and data must be concrete, numbers must be associated with symbols known as \textit{numerals} if they are to be used in computation.

## Semiotics, Language, and Code

Types of sentences - declarative and imperative
An algorithm as an argument

Computation requires communication
Model of communication
All information is encoded and decoded (digital and sensory)

Constructed languages, a subset of which are formal
Trade language, lingua franca, Latin
Leibniz - Alphabet of human thought, "best of all possible worlds," panglossianism

### Writing Systems

Symbol - syntactic, general term
Glyphs - syntactic, a graphical representation
Characters - semantic, associated with meaning (in computing, it refers to an "encoded character" that is represented by a glyph), a unit of information (which is interpreted by means of a type)
Graphemes - the smallest unit in a writing system, a written symbol that represents a sound or phoneme (a logogram, a syllabic character, a letter)
Writing systems - ideographic/pictographic systems (Emoji), logographic system, syllabaries, segmental scripts, alphasyllabaries

Quipu, number systems
Non-linear alphabets, flag semaphore, animal communication
Character encodings
ASCII
Westernism - Scientific Revolution, alphabet, character, terms and jargon in English (covered in greater detail later)
Unicode, code points for abstract characters, UTF-8

### Numeral Systems

and these numbers can be \textit{encoded} with either a single \textit{symbol} or a sequence of symbols called a \textit{string}. For example, the number eight is typically encoded with the symbol 8, which is a \textit{numeral} or \textit{digit}. The number could just as easily be represented by the symbol \varstigma, but this would be non-standard. Numbers are usually encoded according to an established \textit{numeral system} of some \textit{base} or \textit{radix} that specifies how many unique symbols are used for representation. Numerical data intended to be read by humans are typically encoded in a base-10 system, one of ten digits. \\

This design choice is ancient and natural. It is based on the ten digits of our hands, which have aided us in counting for hundreds of millennia. In fact, fingers are the oldest counting tools used by man, and we still use them today for this purpose. Other anatomically inspired bases have been used in early numeral systems, such as base-20, which counts the fingers and the toes, or base-12, which uses a thumb on one hand to count the bones of the other four fingers. However, today, the base-10 \textit{Hindu-Arabic numeral system} is universal in mathematics. \\

The base-60 system of Babylonian numerals is also notable. Its base is thought to have been chosen for its many factors, as this simplifies the process of division. Under this interpretation, this system is \textit{constructed} rather than natural. Instead of mirroring something concrete like physical extremities, this system chooses an abstract base in order to make a procedural optimization. The reasoning for base-2 encoding in computing is similar. It sacrifices human familiarity for performance and reliability. \\

