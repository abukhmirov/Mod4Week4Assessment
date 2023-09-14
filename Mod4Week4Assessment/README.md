# Week 4 Assessment

### Setup
* Fork and clone this repository
* Open your forked repo in Visual Studio.
* Complete the two exercises and the questions

## Exercise 1: Inheritance and Dependency Injection (8 points)

Open up `Program.cs` and run your program. It should run with no errors, if you get an error reach out to your instructor.

This exercise involves some refactoring and some new features.

**Step 1:** Currently there are two classess `Student` and `Teacher` that have a lot of repeated code between them. Create a new class `Person` that will be the base class. Then update `Student` and `Teacher` to be derived from `Person`. Include as much in your `Person` class as you can to keep your code DRY (Don't Repeat Yourself). 

**Testing Step 1:** Uncomment the code under "Step 1:" in the Main method. That code should now run without error.

**Step 2:** Implement a new class called `School` that uses dependency injection and takes in a list of people as a dependency. Implement a method called `ListBirthdays` in your school class that calls the `GetBirthday` method and prints to the console each student and teacher's birthday.

**Testing Step 2:** Uncomment the code under "Step 2:" in the Main method. That code should now run without error and output a bunch of names and birthdays.

Ungraded extra challenge: If you have time, improve the way the birthdays are output. Can you group them by month or by Student/Teacher?

### Exercise 2: Interfaces (4 points)
Open up `InterfacePractice.cs`. You should not need to run this file, you will just edit it.

**Step 1:** Take a look at the two classes `Car` and `Bicycle`. They both implement an interface called `InterfaceNameHere`. Replace all three uses of `InterfaceNameHere` with a fitting name for this interface.

**Step 2:** The interface has already been created for you on line 5. Fill in the details for any methods and/or properties that make sense based on the two classes implementing this interface.

## Questions (8 points)

Edit this file with your answers.

1. What are some of the benefits of using inheritance? (1 point)
    * < Inheritance allows for cleaner, more readable code that can reuse code from the Parent class
	without rewriting it again and again. It also allows for organization and hierarchy. It shows organized 
	relationships between classes and between other objects, making the code easier to understand.>  
2. What might be some of the disadvantages of using inheritance? (1 point)
    * < Inheritance can lead to Inheritance Bloat where the Parent class has too many methods and properties
	and some of the Child Classes may inherit some that they don't need to use. Also testing can be harder with
	inheritance since you would need to test both the behavior of the Parent class and the specific
	behavior of the Child classes>  

3. How would you describe the difference between the base class and the derived class when working with inheritance? (1 point)
	* < The Base class is the origin of the inherited properties and methods, while the derived classes are recieveing them.
	The Base class properties and methods can also be added upon by the derived class.>  

4.  What happens if you define the same method in the parent class and the child class? (1 point)
	* < This can lead to either method overriding or method hiding. If you include the override keyword the Child class will override the Parent method, but if you use the new keyword it will lead to method hiding where the Child method does not override the Parent method, but has its own method details.
	If no keywords are used, you will get a warning about using the same name. This is called method shadowing.> 

5. In your own words, how would you define an Interface? (1 point)
    * < An Interface is a set of rules or a contract that the class that implement it must abide by. They must have the properties and the methods defined by the Interface included in them. > 

6. Does a class implementing an interface need to implement all of the methods in that interface? Why or why not? (1 point)
    * < Yes, the class needs to have all the methods and properties defined in the Interface to fulfill the contract. > 

7. Both Inheritance and Interfaces use the `:` symbol after a class name. If you're looking at a class, what's one thing that can help you determine if the class is implementing an interface of extending a base class? (1 point)
	* < The Interfaces usually are named with IName structure and can usualy be found that way. Also in C# there is no multiple class inheritance, but there is multiple interface inheritance. If you see two objects after the ":" separated by a comma, then those are interfaces.>  

8. If asked in an interview, how would you describe the purpose of the IOC container in a .NET application? (1 point)
	* < Inversion of Control (IOC) containers helps with Dependency Injection and all of the benefits that it provides. IOC containers store and manage the dependencies created in the program. >  


## Rubric

This assessment has a total of 20 points.  A score of 15 or higher is a pass.

As a reminder, this assessment is for students and instructors to determine if there are any areas that need additional reinforcement!
