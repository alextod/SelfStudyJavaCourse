1.	
..*everything is an object – it can save data, and you can ask it to do some operations over itself
..*Program is a group of objects, that talking with each other using messages.
..*Each object has memory consist from another object – you can put any object inside other object
..*Each object has a type – each object is instance of class
..*Every object of specific type can receive the same messages
2.	Class is abstract Data type. But object is specific copy of class. Similar objects which different only with internal state are related to one class.
3.	Characteristics – data elements (group of internal variables). Behavior – functionality of object, what kind of messages, object can operate.
4.	Interface – define what kind of messages you can send to specific object.
5.	Our classes\objects provide a service for client developers. Such way of thinking very help not only during design, but also for reusing objects. You can understand the value if object based on service it provides.
6.	Two reasons for hidden implementation:
..*First – hide the part that shouldn’t be touched by client programmers
..*Second – Change our code without impact on client programmers
Keywords: private, public, protected.
7.	Composition (has-a) – when your new class contains existing classes as a members. These member are private for whom are using this new class.
Inheritance – your new class consist of old class + some modification. To reuse existing functionality and not write it from the beginning each time.
8.	“Is-like-a” -    When you add new interface elements to a derived type. 
Problem that your new type is similar to based type, but new methods are not accessible from based type. So you can send messages which can’t be operate by this type.
9.	polymorphism - the ability to use the methods of the object of a derived class that does not exist at the  time the base class creation
10.	Upcasting - transformation up the hierarchy. From the derived classes to base classes.
The idea is that you can create a dozen heirs in class. Completely different.
Convert them to the type of the base class. Put them together in an array and call the base class methods. This will be called the methods from derived classes.

Downcasting - conversion down the hierarchy. From the base type to the concrete.
Done manually. The programmer should be aware that the pointer actually points to a specific type, not the base.