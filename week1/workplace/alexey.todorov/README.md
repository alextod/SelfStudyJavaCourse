1.	Smalltalk characteristics
	- Everything is and object. Every entity of the program can be presented as an object. Some kind of container with it's on properties and abilities.
	- Program is a group of an objects communicating by the messages. These containers are connected with each other for one certain purpose.
	- Every object has it's own memory consisted of other objects. Each object can contain other objects.
	- Every object has a Type. Type defines the properties and abilities of the object.
	- Every object of the certain type can receive the same messages. The objects of the same type can be treated the same way. For example if the Dog named Limo likes to eat chicken, then the other Dog named Bim likes chicken too.
	
2. The concept of Classes allows us to define our own type of object with it's specific behaviour and characteristics. And object's Data Type is the individuality of the object.

3. We can call the class fields, defining what the class is, as Characteristics of the object. And the methods of the class, defining what the class can do, we can call the Behaviour.

4. Every Data Type has entry points (as the levers or buttons) we can use to get the defined action provided by this Type.

5. "Service Provider" by Bruce is an ability of the object to provide one certain service. This means that one object of one certain type will serve for one purpose. This atomization of the object abilities improves the cohesiveness and usability.

6. The main reason of the hidden implementation is to hide internal, private processes of the class from the public interface for security and usability purposes.
We can use access identifiers "private", "protected" or default "package private" to achieve hidden implementation.

7. Inheritance is when we can consider one class as the part of the other class(is-a relationship), like class Square is a child of class Figure. Composition is when we consider one class has another private class, as the Car class has an Engine class.
Inheritance allows programmer to extend base class and override base methods. Composition allows to use the methods of base class and add additional.

8. a-like-as relationship tells us that two classes can have the same base class but with different methods for example class Motorcycle and class Bicycle have bas class Vehicle but motorcycle has ability to use fuel.

9. Polymorphism allows us to use the same method for different classes and this method will do the certain action for the certain class. For example we have class Figure with method draw().
Then we make two child classes Square and Triangle. Both have inherited method draw(). But in Square we can override it to draw square and in Triangle we override draw() to draw triangle.

10. Upcasting allows programmer to treat subclass as the base class. Downcasting must be done manually and it allow to use base class as subclass.
Example:
Triangle tr = new Triangle();
Figure obj = tr; - upcasting
Triangle tr2 = (Triangle)obj; - downcasting