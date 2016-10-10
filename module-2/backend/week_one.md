## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
GET to get info from the server
Post to send info to the server
DELETE to erease an entry in the server
PUT replace entry in database
PATCH modify an entry in the database

2. What is Sinatra?
A lightweight web server app

3. What is a wireframe and why/when should we wireframe?
Mock sup how you/client thinks a page should look. Useful to discuss the look of your site. 

4. What is MVC?
Model View Controller

5. What's the purpose of having a `Task` model in our `TaskManager` application?
To be able to make instances of Task. 

6. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
It follows REST conventions and is also how Rails works with REST. 

7. What types of variables are accessible in our view templates without explicitly passing them?
Instance 

8. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    erb :index
  end
  ```
  @count = 1

9. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
:locals => {:name => 'Mr. Ed'}

10. What's the purpose of ERB?
to be able to execute Ruby within an HTML view. 

11. Why do I need a development AND test database?
You dont want to be working with actual data when designing the database and site. 

12. What's responsive design?
able to show info on the screen regardless of how big it is. 

13. What is CRUD and why is it important?
Create, Read, Update, Destroy. It is a basic convention of web design. 

14. What does HTTP stand for? 
Hyper Text Transfer Protocol.

15. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
<%= %> renders to the screen. <% %> evaluates ruby code but does NOT render to screen. 

16. What's the difference between unit and feature tests?
Unit is testing the class. Feature is testing that the web page responds the way you are expecting. 

17. How does Capybara help us test our features?
it allows us to "click" on links, ensure that info in displayed, and make sur the page renders the correct way. 

18. What is Nokogiri? When do we use it?
The basics of what Capaybara uses. 

19. How do you know what to test within your application?
Routes, methods, links, etc. Anything that the user needs to look around and most things we make. 

20. What's an ORM?
Object-relational mapping

21. What's the most commonly used ORM?
Active Record

22. What are the benefits of storing data in a relational database rather than YAML or a text file?
You can more easily call data and make connections within your database. 

23. Let's say we have an application with restaurants. There are seven verb + path combinationsnecessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
GET '/restaurants' - to view all restaurants.
GET '/restaurants/:id' - to view a specific restaurants
GET '/restaurants' - to view a form to add a new restaurants
POST '/restaurants' - submit the new info to add the restaurants
GET '/restaurants/:id/edit' - See a form to edit a restaurants's info 
PUT 'restaurants/:id' - Edit the restaurants's info 
DELETE 'restaurants/:id' - delete a restaurants's entry. 

24. Name one exciting/fun/cool/awesome thing you can do with SQL.
Average the column's data.

25. Write an example of the above exciting/fun/cool/awesome thing.
Payload.average("responded_in")
