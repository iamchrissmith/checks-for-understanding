## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
GET - Request something from the server
POST - Send information up to from the client to the server
PUT - Update information received by the client by posting it back to the server
DELETE - Client requests that the server delete information
2. What is Sinatra?
It is a web application framework that is written in Ruby and allows us to access ActiveRecord and our own homespun MVC
4. What is MVC?
Model, View, Controller:
Model - holds our logic and database objects
View - holds our display for the user
Controller - dictates the routes for the application
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
"Built in" documentation to communicate their purpose to future devs (or future us'es).  Also, it aligns with what we will see in Rails.
6. What types of variables are accessible in our view templates without explicitly passing them?
Instance variables
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    @count = 1
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?
```ruby
  get '/horses' do
    @count = 1
    erb :index, :locals => {:name => "Mr. Ed"}
  end
```

9. What's the purpose of ERB?
ERB allows us to mix ruby into HTML templates
10. Why do I need a development AND test database?
Test DB is for running specs through something like Capybara (i.e. it will get set up and destroyed each time we run specs).
Development DB is for working on the application and running Shotgun
11. What's responsive design?
Adapting a website's design/layout to different viewports (screen sizes)
12. What is CRUD and why is it important?
Create, Read, Update, Delete
Model/framework for us to set our web applications up to interact with databases
13. What does HTTP stand for? 
Hypertext Transfer Protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
`<%= %>` - outputs the Ruby return to the screen
`<% %>` - Runs the ruby without outputing to the screen
15. What's an ORM?
Object Relationship Model - How we tie the database to ruby objects
16. What's the most commonly used ORM in ruby (Sinatra & Rails)?
ActiveRecord
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
| Verb | path | description |
| Get | /restaurants/new | display a form to the user to enter new info about the restaurant |

18. What's a migration? 
19. When you create a migration, does it automatically modify your database?
20. How does a model relate to a database?
21. What's the difference between agile workflow and waterfall method?
22. What is the difference between `#new` and `#create`?
