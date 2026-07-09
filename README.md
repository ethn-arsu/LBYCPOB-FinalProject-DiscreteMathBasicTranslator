# Discrete Math Translator - A Rule-Based English-to-Discrete Mathematics Notation Translator

### TEAM MEMBERS
Ethan Edgar C. Arsua - ethn-arsu

Aeon Alphonse E. Mauricio - foobar-trashdump

Zamuel Paolo L. Robes - zamuelrobes-cmd

### PROBLEM STATEMENT & GOALS
Discrete Mathematics is a core subject in many Computer Studies, Engineering, and Mathematics programs, which are all incidentally offered at De La Salle University (DLSU). This subject is known to be difficult for students to convert English statements into formal discrete mathematics notation, particularly in propositional logic, predicate logic, and basic set theory. The project aims to address this learning gap by providing a rule-based translator that converts supported English sentence patterns to mathematical expressions.

The project aims to:
- Translate supported English statements into discrete mathematical notation.
- Help students understand the relationship between English statements and mathematical symbols.
- Provide a simple, user-friendly educational tool developed with object-oriented programming (OOP) principles.

### TARGET USER
- Information Technology students
- Computer Science students
- Computer Engineering students
- Engineering students taking discrete mathematics
- Mathematics students taking introductory logic and set theory.

### BRIEF DESCRIPTION
The Discrete Math Translator is a Java-based program designed to translate standard English sentence structures into their discrete mathematics equivalents. The application is designed to accept English input (derived from a set of sentence structures) and recognize common logical structures, including conjunctions, disjunctions, implications, and negations.

After the translation, the program displays mathematical notation along with an explanation of which logical rules were found and how they are present in the given sentence. If the entered statement does not match any supported pattern, the application will handle the exception, inform the user which kind of input is accepted by the program, and suggest supported input formats. 

### CORE OOP CONCEPTS
- Encapsulation: The logic components/ translation rules will contain their own internal data and logic. Program objects contain private fields and public methods, allowing controlled access through said methods.
- Inheritance: Different translation rules inherit the methods from a shared parent class.
- Polymorphism: Individual translation implementation between objects is done via overriding the shared methods present, given a parent class. The program will select an appropriate rule at runtime based on user input.
- Abstraction: TranslationRule abstract parent class has methods that define shared behaviors that every translation rule must implement. The main will interact with these rules through the abstract without needing to know the individual implementation of the objects.

### INITIAL CLASS IDEAS
- TranslationRule: Abstract class that serves as the blueprint for all translation rules.
- ConditionalRule: Implements translation for implication statements.
- ConjunctionRule: Implements translation for conjunction statements.
- NegationRule: Implements translation for negation statements.
- TranslatorEngine: Coordinates the translation process by selecting the appropriate rule based on user input.
- Expression: Stores the original English statement, mathematical notation, and generated explanation.
- TranslationResult: Stores the final notation, assigned variables, detected rule, and explanation before displaying it to the user.
- UserInterface: Handles user interaction via JavaFX.

### USER STORIES
- As an engineering student, I want to input an implication statement so that I can instantly see its formal notation.
- As a struggling discrete math student, I want to see a breakdown of the translation process so that I may learn and improve my discrete math skills.
- As a computer science student, I want to know when my input is unsupported so I can rewrite it correctly.

### CORE FEATURES:
- Rule-based pattern matching to recognize supported English sentence structures.
- Translation of English statements into discrete mathematics notation.
- Automatic variable assignment (e.g., P, Q, R) for identified propositions.
- Legend generation that maps variables to their corresponding English statement.
- Step-by-step explanation of how the translation is performed.
- Program feedback for unsupported or invalid inputs.
- 'Supported Formats' reference page containing examples of accepted sentence patterns.
