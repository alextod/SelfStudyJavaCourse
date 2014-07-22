# *Five basic characteristics of the language which represent an approach to object-oriented programming.*
  - *Everything is an object* 
     Object is a fancy variable. It can save some data. We can do request to the object and it perfom operations on itself.
  - *A program is bunch of objects telling each other what to do by sending messages*
    A program consists of objects that can send "messages" each other. If a object got message/request from other object then it has to perform the expected action.
  - *Each object has memory its own memory made up of other objects* 
  Each object has own memory that contains other objects. We can include any objects to other object.
  consist from another object – you can put any object inside other object
  - *Every object has a type*
  Each object is instance of class. Requests that we can send to an object depends on the object type.
  - *All objects of a particular type can receive the same messages*
  Objects that have the same type can receive the same messages.

# *How do you understand concept of classes and objects? What does the “Data Type” term mean?*
Class is an abstract data type. When we use "Data Type" term  we mean entity that has specific data and specific behavior. Object is a variable of class. Instances of the same class have different state and identical functionality.

# *“An object has characteristics and behaviours”, explain how you understand this expression.*
Characteristics – data elements (bunch of internal variables). 
Behavior – functionality of object, what kind of messages, object can operate.

# *When someone points out that any Data Type has an interface. What is implied there?*
Interface is the full list of requests  that you can make for a specific object.

# *Bruce suggests the way of thinking of a program design named “service providers”. Explain how you understand it.
> Hint: mind the “cohesion” term, it’s one of the important measurements of software quality in computer programming.*
Each object provide some service. Object has to do one thing well.
This way of thinking  helps during design a program. 
It makes your code understandable and someone can reuse objects.

# *What are the main reasons to hide implementation? What keywords in Java can be used to achieve the hidden implementation?*
The hide implementations has two reasons:
1st - hide the part that shouldn't be touched by client programmers.
2nd - the class designer can change internal behavior and it will not affect the client programmers.
Keywords: private, protected, public. Java also provide <empty value> that means  "package access".

# *As you already know, there are two classes relationships: Inheritance (is-a relationship) and Composition (has-a relationship). Explain the difference between them, describe advantages/disadvantages of each approach.*

Composition (has-a) – when your new class contains existing classes as a members. These member typicaly are private. We can dynamically change the member object.
This feature makes your program more flaxible.

Inheritance – your new class consist of old class and some changes. It allow to reuse existing functionality.
Inherited class realizes the interface of superclass with some changes. 
Inherited class also can extend functionality of superclass.

# *Bruce stated a “is-like-a” term, it’s a relationship that comes from “is-a” relationship. What is considered there? What problem do you see there?*
Relashioship "is-a"  - when inherited class override only baseclass methods. Inherited class has the same interface and some/all its methods have other realisation.
Relashioship "is-like-a" - when inherited class override baseclass methods and it has some new methods.
The problem: new type(a inherited class) is similar to the base type (the base class), but the new methods are not available from base type.
We cannot use them when you operate with the base type.

# *Explain Polymorphism as you understand this term. Give an example. *
Polymorphism is the opportunity to use different classes independently of their types if they have the same base type.

Example:
My class "SomeClass" has a class DB as mebmer.
Also we have classes MySQL and PgSQL that was inherited from DB.
They realized the same interface.
     DB
      |
   -------
  |       |
MySQL   PgSQL

When we create object of SomeClass we can specify type of db in a SomeClass' constructor.
DB database = new MySQL();
or
DB database = new PgSQL();

Data type of "database" is DB.
When we use it (for example database.showTables() ) will be executed methods from the inherited data type (MySQL or PgSQL).
It occurs due to the late-binding conception.
Also we can change DB type in runtime mode.

# *How do you understand the “upcasting” and “downcasting” terms? Give an example.*

Upcasting - change object's type from the inherited class to base class. Thus, we can work with the object of the derived class as a object of the base class.
Example: DB database = new MySQL(); We create a new object that has MySQL type and assign it to the variable "database" that has type DB.

Downcasting - change object's type from the base class to the inherited class.
