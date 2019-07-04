# Builder Design Pattern

## Intent ([source](https://sourcemaking.com/design_patterns/builder))

- Separate the construction of a complex object from its representation so that the same construction process can create different representations.
- Parse a complex representation, create one of several targets.

## Purpose ([source](https://en.wikibooks.org/wiki/C%2B%2B_Programming/Code/Design_Patterns#Builder))

The Builder Creational Pattern is used to separate the construction of a complex object from its representation so that the same construction process can create different objects representations. 

- Problem - We want to construct a complex object, however we do not want to have a complex constructor member or one that would need many arguments.
- Solution - Define an intermediate object whose member functions define the desired object part by part before the object is available to the client. Builder Pattern lets us defer the construction of the object until all the options for creation have been specified.
