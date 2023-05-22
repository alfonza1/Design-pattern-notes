


Solid Principles - Code Fragility and Technical Debt:
Code Fragility refers to the software's inclination to break in multiple places whenever changes are made. It indicates the lack of robustness and resilience in the codebase.


Technical Debt represents the cost incurred by prioritizing rapid delivery over code quality for extended periods. It involves the trade-off between quick fixes with poorly written code 
(fast delivery) and investing more time in producing high-quality, maintainable code (code quality).


Accumulation of technical debt is an unavoidable consequence, regardless of the team's expertise. If left unchecked, it can significantly jeopardize the project's success.
The key lies in managing and minimizing technical debt.


Solid Principles - Overview and Benefits:
The acronym SOLID stands for Single Responsibility Principle, Open-Closed Principle, Liskov Substitution Principle, Interface Segregation Principle, and Dependency Inversion Principle.
These principles contribute to creating well-designed and maintainable software systems.


The Open-Closed Principle emphasizes the potential risks associated with modifying existing code and suggests that classes, functions, and modules should be closed for modification but open for extension.
Closed for modification means that existing source code remains untouched when adding new features, essentially making the source code immutable.


Changing requirements are inevitable, and to accommodate them without modifying existing components, inheritance and design patterns prove to be effective. 
The Open-Closed Principle also applies to packages. In some cases, modifying a component becomes necessary when extending it is not practical. 
However, designing with flexibility introduces additional complexity.


The Liskov Substitution Principle advises against thinking of relationships solely in terms of "IS A." 
Empty methods, type checking, and stringent preconditions indicate violations of the Liskov Substitution Principle. 
Additionally, the Single Responsibility Principle is applicable to interfaces, not just class inheritance. 
Often, fixing an incorrect type hierarchy requires breaking it, as real-life categories do not always align perfectly with object-oriented programming relationships.


The Interface Segregation Principle (ISP) is connected to the Single Responsibility Principle (SRP) and the Liskov Substitution Principle (LSP). 
It is important not to confuse the term "interface" in ISP with a Java interface. It is crucial to observe symptoms of large interfaces and take appropriate action. 
Breaking large interfaces into focused ones for the code you own is recommended, and when dealing with external code, the "Adapter Pattern" can be utilized.


The Dependency Inversion Principle (DIP) is also linked to the Single Responsibility Principle (SRP) and the Interface Segregation Principle (ISP). Similar to ISP, 
it is important not to mistake the term "interface" in DIP for a Java interface. Paying attention to symptoms of large interfaces and taking necessary measures is vital. 
Breaking large interfaces into focused ones for the code you own is advisable, and for external dependencies, employing the "Adapter Pattern" is beneficial.





Design Patterns:

Design patterns are reusable solutions with specific names that address recurring problems within a given context.
They capture expert knowledge and facilitate knowledge reuse.
They guide the selection of appropriate designs and promote a shared and precise vocabulary.
OOP Principles:

SOLID (Single Responsibility, Open-Closed, Liskov Substitution, Interface Segregation, Dependency Injection):
These principles define important aspects of object-oriented programming.

Favor composition over inheritance:
It is recommended to prioritize composition as a more flexible alternative to inheritance.

Programming to interfaces:
Emphasizes the importance of designing code to interface specifications.

Pattern Classification:

Purpose:
Patterns are classified based on their purpose, such as creational, behavioral, and structural patterns.

Scope:
Patterns can be classified based on their scope, whether they apply to classes or objects.


Examples of Design Patterns:

Singleton:
Ensures a class only has one instance and provides a global point of access.

Factory Method:
Allows subclasses to decide which class to instantiate.

Abstract Factory:
Creates hierarchies or families of related objects.

Builder:
Separates the construction of an object from its representation.

Facade:
Simplifies an interface to a subsystem, decoupling a client from it.

Decorator:
Attaches additional responsibilities to an object dynamically.

Adapter:
Converts the interface of a class into another interface expected by clients.

Proxy:
Provides a surrogate for another object to control access to it.







Chapter 11

Abstract Classes:

Abstract classes are declared by using the "abstract" keyword.
If a subclass extends an abstract class, it must implement its abstract methods or become an abstract class itself.
Abstract classes cannot be instantiated; they are designed to be used as superclasses.
Interfaces:

Interfaces cannot be instantiated directly.
When a class implements an interface, it must implement all the methods defined in that interface.
If a class does not implement all the methods, it must declare itself as abstract.
Abstract Methods:

Methods within an interface can be declared as abstract explicitly or as default.
Abstract methods lack an implementation and require explicit declaration.
Default methods provide a default implementation within the interface.
Overall, abstraction in test automation involves using abstract classes and methods as templates, implementing them in subclasses, 
and adhering to the rules regarding abstract classes, interfaces, and abstract methods.



Chapter 13a - b: Exception Handling
An exception refers to an unforeseen event that occurs during runtime due to an error in the program's execution.

Exceptions can be managed using the try/catch construct. When an exception is caught, it can be accessed through the stack trace and the getMessage() method, which provides the error message without the stack trace.

The finally block is employed to execute code that should always run, regardless of whether an exception is thrown or caught.

The "try with resources" feature allows for automatic closure of resources without explicitly using the finally block. This feature requires the resource to implement either the Closable or AutoClosable interfaces.

If a method contains code that may throw an exception, it must handle the exception using try/catch or propagate it by specifying the exception type using the throws keyword in the method signature.

The throws keyword is utilized to declare the type of exception that a method may throw.






