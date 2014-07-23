1.
  - Everything is an object.  Every physical or abstract item in the world can and must be  presented into specific way in OOP laguages.
  - A program is a bunch of objects telling each other what to do by sending messages. Have no idea what to add here
  - Each object has its own memory made up of other objects. You can create new object by combaining functionality of other objects. 
  - Every object has a type. Every object has its class  accessory.
  - All objects of a particular type can receive the same messages. Even if  objects can belong to different class but the same type - they still can received some of the messages from each other.
  
2.
 Clases discibes what your code can do and in which state it can  be (this is a data type). The object is an conrete copy of the class with concrete state.  
  
3.
 Characteristics is the state (the number of fields and their values) of the Class.
 behaviours  is the functionality covered by the methods of the Class.
 
4.
 While behaviours is just a vector of runctionality interface is a concrete list of methods that your class need to be able to execute.
 
5. 
 Your entire program  should provide the list of services that is required from customers. Best way to accomplish that is to split this list of services to different objects. 
 So each object should provide some services : from the needed list or to help other objects to accomplish that. 
 Because of that - each of your objects should not do all at once. Split the functionalty beetwen objects so you can use them in future.
 
6.
 We need some rules here, ok? If you don't want to someone see your impelemntation (shitty coding or something else) - hide it. 
 It will be easier for other devs to see - are they allowed to change something in your implementation or not.
 Also in future it will be easier to refactor your hidden code - because nobody is working with its implementation. Other devs are working with services that your objects are providing.
 The main keyswords that you need to know - public, private, protected. If you don't mark you code with one of these words - it will get default status(allowed in the package)

7.
 Composition means that you are using other objects inside a new object. It's the great example of reusing already written code.
 Inheritance means that new class is created with additional and overrided functionality of its parent. So you don't need to create a needed class from scratch. 
   These 2 classes will have the same type - so a lot messages can be send beetwen them.

8.
 If you use isALike relationship your child class has more functionality than the parent. But they are still of the same type which can lead lead to problems of non reacheble methods sometimes.

9.
 This is actually a some kind of magic. Thanks to the late binding you can no worry about the question if the right method of child classes was executed.
 It you want to all animals in your animal array to make sound - just call makeSound() . Dogs will barks and cats will meow. Not sure about the foxes.
 
10. Updasting - change the object type from child to parent. So you will able to work will huge amount of objects in the same way.
	Downcasting - change the object type from parent to child. You need to do that, if some objects need to execute childish methods.
	
	 
 