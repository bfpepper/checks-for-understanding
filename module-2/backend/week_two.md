## Week Two - 1606-BE Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
  It is an ORM It allows us to "talk" with the database ad send SQL commands without writing SQL commands
2. What is a migration?
  It allows us to create/modify a table with given attributes. 
3. How does a table relate to a model?
  the model is the class of the given table. it allows us to make not only methods to call on a modle but alos set up relationships to       other models. 
4. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
  class methods A horse can belong to a stable and a stable has many horses. 
5. What do they allow you to do?
  to set up the relationships between classes.
6. What's the difference between agile workflow and waterfall method?
  Agile is more flexable and able to abapt to client needs. Waterfall is the antitisis of that. 
7. What is the difference between `#new` and `#create`?
  New makes a new instance of that class but does not save it to the database. Create does both. 
8. At a basic level, what does cURL allow you to do?
  Send HTTP requests to a server without using a broswer.
9. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
  STUDENTS       TEACHERS
  id
  name           name 
  age            class
  teacher_id     id
10. Define foreign key, primary key, and schema.
  primary key is the unique identifier that id's an instance. A foreign key sets up a relation between a given class and a class it         'belongs' too. 
11. Describe the relationship between a foreign key on one table and a primary key on another table.
  The foreign key on one table points to the prmary key of the other. 
12. What are the parts of an HTTP response?
  response code and the response headers. 
13. `Rack::Test` allows us to test our controllers in isolation. What are some of the methods it gives us to simulate the request/response cycle?
  All http verbs are methods that let us simulate a request
14. Describe some techniques to make our Sinatra views more DRY. Give an example of when you would use these techniques.
  Use partial views when two or more views have the same code. if there is logic in the view, break it out into the appropriate class. 


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
3. What's the difference between agile workflow and waterfall method?
  see question 6 above
4. What can you expect from a group as you begin working together? As you continue working together?
  Forming, norming, storming, preforming
5. What two columns does `t.timestamps null: false` create in our database?
  create_at and updated_at
6. What cURL flag can you use to send a `POST` request?
  -p
7. What case does JSON (and JavaScript) use for multi-word variables?
  camelCase
8. What case does Ruby use for multi-word variables?
  snake_case
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
  in the traditional school system, a teacher would belong to a school and a scholl has many teachers. 
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
  SCHOOL      Teacher
  id          id
  name        name
  teacher_id  
  
11. Give an example of when you might want to store information besides ids on a join table.
  If the join tbale has data unique to that table that does not need to be on other tables. 
12. Describe and diagram the relationship between patients and doctors.
  for elderly amercians, a patient has many doctors and a doctor has many patients
13. Describe and diagram the relationship between museums and original_paintings.
  a museum has many paintings and a painting belongs to a museum
14. What are some examples of acceptable values for the parts of an HTTP response?
  Headers, and content
15. What types of output do we want to test when we test our controllers? 
  that the controller is sneding back the correct response given the parameters
16. What could you see in your code that would make you think you might want to create a partial?
  repeated code for create and update. 
17. Why might you use a helper method?
  to clean up the logic oin the controllers. 
