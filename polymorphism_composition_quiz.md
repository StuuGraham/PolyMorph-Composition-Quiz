# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

To make many changes ('poly' - many, 'morphism' - change, from Greek)
Polymorphism is used through Interfaces or Superclasses in Java coding.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

It means we are writing numerous classes that all share and use a common Interface, with each class being able to have its own unique version of the Interface and its functions if required

3. What can we use to implement polymorphism in Java?

Superclasses or most commonly Interfaces

4. How many 'forms' can an object take when using polymorphism?

An object can only have one Superclass, however it may utilise as many Interfaces as we see fit.

5. Give an example of when you could use polymorphism.

If we were to be building an app that gave us different lists of various different sports players, an 
Interface, IPlay may be implemented. There could be a FootballPlayer Superclass with various different
positional classes branching off as well as a RugbyPlayer Superclass with its own various different classes 
for individual positions, however they all at some point in a game would want to kick a ball or run and so on, 
so they could all utilise the IPlay to handle these common functions, whilst still having unique functions to 
their sport within the Superclasses.

# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

Composition is when an instance variable or class is built with a reference to another instance variable or class.

7. When would you use composition? Provide a simple example in Java.

We would use this when we want to model something like a Library. There would be a Library class, and a Book class, possibly even a LibraryMember class or such. The Library however would have it's BookCollection be dependent on having an ArrayList of Books and possibly an ArrayList of Members as well, this means the Library class is dependent on these Classes, or could be referred to as composed with them.

8. What is/are the advantage(s) of using composition?

It allows the reuse of already written code (DRY). Java doesn't support multiple Inheritance, but this is a way to circumvent that. Composition makes testing easier.

9. When an object is destroyed, what happens to all the objects it is composed of?

They are also destroyed. In my example above, if the Library instance was destroyed, so would all the instances of Books and Members it was composed of.