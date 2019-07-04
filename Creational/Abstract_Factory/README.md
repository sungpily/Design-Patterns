# Abstract Factory Design Pattern

## Intent ([source](https://sourcemaking.com/design_patterns/abstract_factory))

- Provide an interface for creating families of related or dependent objects without specifying their concrete classes.
- A hierarchy that encapsulates: many possible "platforms", and the construction of a suite of "products".
- The new operator considered harmful.


## Definition ([source](https://en.wikibooks.org/wiki/C%2B%2B_Programming/Code/Design_Patterns#Abstract_Factory))

A utility class that creates an instance of several families of classes. It can also return a factory for a certain group.

The Factory Design Pattern is useful in a situation that requires the creation of many different types of objects, all derived from a common base type. The Factory Method defines a method for creating the objects, which subclasses can then override to specify the derived type that will be created. Thus, at run time, the Factory Method can be passed a description of a desired object (e.g., a string read from user input) and return a base class pointer to a new instance of that object. The pattern works best when a well-designed interface is used for the base class, so there is no need to cast the returned object.

- Problem - We want to decide at run time what object is to be created based on some configuration or application parameter. When we write the code, we do not know what class should be instantiated.

- Solution - Define an interface for creating an object, but let subclasses decide which class to instantiate. Factory Method lets a class defer instantiation to subclasses.
