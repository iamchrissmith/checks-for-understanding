## Week One - Module 4 Recap

1. What's the most useful thing you learned from completing the intermission week work?

I liked working through the Express REPL exercises.

2. What are some tools to help debug JavaScript code?

- Debugger
- Console (in browser)
- PryJS

3. What are some tools you need in order to unit test your JavaScript?

- Mocha
- Chai
- NPM / Webpack

4. What is the syntax for invoking a function?

`()`, so if you have a function like:
```javascript
function() {...}
```
It gets invoked when the file is run. However, if you have:
```javascript
const myFunction = () => {...}
```
You have to call `myFunction()` to invoke the function.

5. What is CORS?

It stands for Cross-Origin Resource Sharing and has to do with allowing external JS resources to affect the current page.

6. How do we enable CORS?

You have to tell the receiving server to allow the specific methods in the header.

7. What's `this` in JavaScript?

`this` in JS is hard...  
Roughly, it is the `self` and is scoped to the current object.  On the root scope, it is the document.  Inside a class or function it is the class or function.  In ES6 arrow functions it is the function's parent.  

8. What is Webpack and why is it useful?

Compiles, concatinates, and minifies our JS (and CSS) files.  It allows for easier file management and local development. 

9. When/why do you want to use event delegation?

So that you can apply events to elements that were not in the DOM when the page/JS was loaded.

10. What is a callback function?

The function that receives the call from an action or other function.  I.E. `$(...).on('click', myCallBackFunction)` receives the `event` from the click action.

11. What's `npm` and what do we use it for?

Node Package manager.  We use it like `gem` to install and manage our javascript packages.

#### Review  
12. What's the MVC design pattern? Describe each part of MVC.

Model: Handles the logic and data  
View: Handles display  
Controller: Handles connecting the Model to the View and receives Routing.  

13. What are a few ways to optimize a Rails application?

Caching and efficient database/ActiveRecord calls

14. What's a background worker? When would we want to use a background worker?

A process that executes a job outside the normal page load of our app.  This allows for sending complex or asyncronous tasks to the background while the user can move on and do other things.
