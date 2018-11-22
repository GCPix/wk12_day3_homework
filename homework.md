Polymorphism
What does the word 'polymorphism' mean?
something that comes in many forms

What does it mean when we apply polymorphism to OO design? Give a simple Java example.
In terms of OO design it means we can give an object, method or variable different meanings or values in different places.
in terms of Java we could have an Attack() method.  How they attack and what they are allowed to attack could be different but it is the same method called.
What can we use to implement polymorphism in Java?
You can use an interface or abstract class/method

How many 'forms' can an object take when using polymorphism?
As many as you want?

Give an example of when you could use polymorphism.
When you have a superclass that holds properties and methods for a particular screen but based on a type of user the functionality changes.  If I had a screen showing someones details an Admin subclass would have a view() method that allows them to see all information other than 'sensitive'.  An SMT subclass would use the same view() method to see all details including the sensitive and a Teacher might only see some details and no sensitive information.  I might have an abstract method view() on a Role superclass.
Composition
What do we mean by 'composition' in reference to object-oriented programming?
it is a 'has a' relationship with the main class.  basically you have an instance of the class as a field inside the constructor on the class you want to use it in

When would you use composition? Provide a simple example in Java.
When the thing you are making up is made of multiple other objects. A fridge has a heat exchanger, has a light, has shelves, has coolant all of which need to be in the Fridge class.  We can pass each object as a variable and then call the methods that are specific to them.

What is/are the advantage(s) of using composition?
The classes are independent therefore the risk of a change in the class being brought in breaking everything is reduced.
it allows methods to be written where they are needed ie I wouldn't want a rotate method on a radio component but I would on a tyre component.  If I using composition Tyre tyre; I can do tyre.rotate() but Radio radio will not allow me to do radio.rotate()
You can test whether this works as you go with TDD
I think it is a way to get around the fact Java does not allow multiple inheritance?
