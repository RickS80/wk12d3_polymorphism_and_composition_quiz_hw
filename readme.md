WHAT DOES THE WORD 'POLYMORPHISM' MEAN?

Polymorphism comes from the ancient Greek words 'poly' and 'morphe' meaning many forms.


WHAT DOES IT MEAN WHEN WE APPLY POLYMORPHISM TO OO DESIGN? GIVE A SIMPLE JAVA EXAMPLE.

Polymorphism means that we can put several objects into an enclosing type that defines a contract between them all. This can be done in Java by using
(abstract) classes and/or interfaces.

An abstract class act as a super-class which sub-classes can inherit from.

Interfaces allows us to treat a class as having another 'type'. One benefit of interfaces is that a class can implement multiple interfaces vs abstract
class where each class can only ever have one abstract superclass.


WHAT CAN WE USE TO IMPLEMENT POLYMORPHISM IN JAVA?

We can use abstract classes and interfaces.


HOW MANY 'FORMS' CAN AN OBJECT TAKE WHEN USING POLYMORPHISM?

Abstract classes - one abstract class can have multiple subclasses. However a subclass can only extend one superclass.

Interfaces - classes can implement multiple interfaces.


GIVE AN EXAMPLE OF WHEN YOU COULD USE POLYMORPHISM.

Polymorphism allows code to be both dry and scaleable which is best practice for large codebases.

COMPOSITION
WHAT DO WE MEAN BY 'COMPOSITION' IN REFERENCE TO OBJECT-ORIENTED PROGRAMMING?

Composition refers to 'HAS A' principle of classes rather than looking at a class in terms of 'IS A'. i.e. a class is composed of elements such as a hotel is composed of rooms, or a car is composed of an engine.

Composition allows a class to use a behaviour common to other classes.


WHEN WOULD YOU USE COMPOSITION? PROVIDE A SIMPLE EXAMPLE IN JAVA.

Often inheritance does not scale well and gets messy, thus using composition tools such as interfaces will assist.

Setting up an inheritance will mean that multiple classes can access the same behaviour. An example would be a wizard with several 'IFlyable' objects such
as a magic carpet, broomstick or dragon. Each of the objects would get the 'fly' behaviour from interface 'IFlyable' although they would otherwise be
different.

WHAT IS/ARE THE ADVANTAGE(S) OF USING COMPOSITION?
Classes can implement multiple interfaces whereas they can only extend one inheritance
Code becomes dry and scalable as the behaviour can be used across multiple classes that are otherwise different
We can swap in and out these behaviours at run time
Using an abstraction which low level modules can implement makes the code extendable.

WHAT HAPPENS TO THE BEHAVIOURS WHEN THE OBJECT COMPOSED OF THEM IS DESTROYED?
If a low level object is destroyed, it will make no difference to the behaviours. There may be other objects that use
the same behaviours and these would not be impacted.
There would however be an issue if the behaviour itself was deleted. The object would be destroyed.
