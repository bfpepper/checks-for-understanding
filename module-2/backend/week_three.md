## Week Three Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What are the 3 main features in an ERD?
2. Create an ERD for the following database: Restaurants, Customers, Items, Ingredients, Beverages, Orders, Vendors.
3. What is the entry at the command line to create a new rails app?
    rails new *Project name*
4. What do Models generally inherit from in rails?
    ActiveRecord::Base
5. What do Controllers generally inherit from in a rails project?
    ApplicationController
6. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
  get "/horses/:id", to horses#show
7. What rake task is useful when looking at routes, and what information does it give you?
    rake routes; shows you the helper name, method, URI pattern, and controller action
8. What is an example of a route helper? When would you use them?
    artist_path (the _path portion). makes it so instead of hard coding your paths they are dynamic and easier to change in the future
9. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
    _url is the who url (starting with http...) and _path is the relative path given the root URL.  
10. What are strong params and why are the necessary?
    they are there to ensure that only those params get passed through to the DB. without the safe guard someone could interject different parmams.
11. What role does `form_for` play in helping us create our forms?
    is a method that allows us to easily create the necessary fields and buttons for our submitting pages.
12. How does `form_for` know where to submit the user's input?
    Magic
13. Create a form using a `form_for` helper to create a new `Horse`. 
    form_for(@horse) do |f|
      <%= f.label :name %>
      <%= f.text_field :name %>

      <%= f.label :breed %>
      <%= f.text_field :breed %>

      <%= f.submit %>
14. Why do we want to validate our models?
    for many reasons. Mostly to ensure that the new entry is not submitted to the DB without being completly filled out. 
