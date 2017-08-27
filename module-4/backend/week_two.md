## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's one difference between ES5 and ES6?

ES6 is moving JS to more natively support OOP.  One instance of this is the new Class structure.

2. What's the difference between asynchronous and synchronous JavaScript? 

synchonous JS runs all at once where as asynchronous allows us to tell the program to run Y line of code after X has happened successfully.

3. What are the four pillars of Object Oriented programming?

Abstraction - only show the outside world what is needed for it to interact with an object.  
Polymorphism - can redefine functionality by reusing a name  
Inheritance - create and share code through relationships between classes  
Encapsulation - bind data and functions together in one class  

4. What are some tools available in JavaScript to help you write object oriented code?

`Class`es `static` methods and instance methods.

5. What are some key concepts to be aware of when refactoring your JavaScript?

Watch for code smells, follow SRP, watch for async problems/nested callbacks.

6. What's a callback function and what are some reasons when we use/need callback functions?

A function that gets called from another function when the first is finished executing.  It is a way of chaining actions to create asycronicity.

7. What's the scope of variables in Javascript?

Variables are scoped to their containing closure in JS.

8. What's the difference between `==` and `===` in JavaScript?

`===` checks type as well as equality.

9. Why do front end frameworks exist?

To make it easier to do things in JS.  What would take a line in jQuery might take 10 in vanilla JS.

#### Review  

10. Why do people say "HTTP is stateless"?

Each new request is fresh.  It does not store any memory of the past.

11. Describe a RESTful API.

It is an API that adheres to a specific structuring convention for standard CRUD functions.

12. What are some main characteristics of a team following an agile workflow?

Sprints, flexibility, standups.

13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?

OAuth can be complicated to setup and relies on a third party service for authentication.  However, it can streamline your authentication process and 'outsource' the security of it to a more capable actor.
