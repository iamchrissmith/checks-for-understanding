## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. At a high level, what is Node?

Node is a backend language written in JavaScript usually used for servers.

2. What is Express? Why is Express similar to in the Ruby world?

Express is a framework for Node projects

3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.

```javascript
const express = require('express');
const router  = express.Router();

router.get('[PATH]', [CALLBACK]);

```

4. What do we use Knex for?

Database queries.  It is similar to ActiveRecord.

5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?

Create a routes file which uses callbacks that are stored in the Controller files which call on Model files to make database queries.

6. How do you execute raw SQL in node?

```javascript
database.raw(
      [RAW SQL]
    ).then(data => data.rows);
```
Where database is the knex object you configured to connect to your database.

7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?

Advantages: 
* You can have different teams working on the project.
* Your backend can be an API that serves multiple frontends (e.g. mobile app, website)
* better seperation of concerns (i.e. you can use the best tools for frontend and backend and mobile rather than the best tool that does all three)

Disadvantages:
* You app has to interact only with API call.  Which can complicate authentication, authorization, and increase load times.
* more server environments to manage

#### Review  

8. Describe DNS.

Domain Name Servers.  These store IP addresses and match them to URIs to route internet traffic.

9. What does writing clean code mean to you?

Code that is easy to understand what it does and is easy to maintain and extend.

10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?

Hotel - Master class, communicates and tracks other classes. Also stores data about the hotel as a whole  
Room - stores its details and availability
* This could be an inheritance structure where we have a parent room class and then child classes for sleeping rooms, conference rooms, public rooms, etc.
People - perhaps we need to model staff, owners, etc.

