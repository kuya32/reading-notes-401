# Read: 08 - OO Design

## SOLID principles intro

- S.O.L.I.D is an acronym for the first five object-oriented design principles
  - S - Single-responsibility principle
  - O - Open-closed principle
  - L - Liskov substitution principle
  - I - Interface segregation principle
  - D - Dependency Inversion principle
- Single-responsibility Principle (S.R.P)
  - A class should have one and only one reason to change, meaning that a class should have only one job.
- Open-closed principle
  - Objects or entities should be open for extension, but closed for modification
- Liskov substitution principle
  - Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T.
  - All this is stating is that every subclass/derived class should be substitutable for their base/parent class.
- Interface segregation principle (I.S.P)
  - A client should never be forced to implement an interface that it doesn't use or clients shouldn't be forced to depend on methods they do not use.
- Dependency inversion principle
  - Entities must depend on abstractions not on concretions. It states that the high level module must not depend on the low level module, but they should depend on abstractions.

## OO SOLID principles in real life

- S is for Single Responsibility Principle (SRP)
  - Asserts that a class or module should do one thing only.
  - Reinforced with the heuristic that the class or module should have only one reason to change.
- O is for Open/Closed Principle
  - States that code entities should be open for extension, but closed for modification.
  - You should write a class that does what it needs to flawlessly and not assume that people should come in and change it later.
  - Example in real life:
    - Smartphones
- L is for Liskov Substitution Principle (LSP)
  - Any child type of a parent type should be able to stand in for that parent without things blowing up
  - Example if you have a class, Animal, with a MakeNouse( ) method, then any subclass of Animal should reasonably implement MakeNoise( ). 
- I is for Interface Segregation Principle (ISP)
  - You should favor many, smaller, client-specific interfaces over one larger, more monolithic interface.
  - Example in real life:
    - Think of going down to your local corner restaurant and checking out the menu. See all of the normal menu mainstays, and then something that's just called "soup of the day." Because the soup changes a lot and there's no sense reprinting the menus every day. 
- D is for Dependency Inversion Principle (DIP)
  - Encourages you to write code that depends upon abstractions rather than upon concrete details.

[Back to README](README.md)
