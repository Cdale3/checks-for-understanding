## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

1. List the five common HTTP verbs and what the purpose is of each verb.
    GET - Usex to retrieve information from the server.
    POST - used to send data to the server
    PUT - Replaces all current content with updated data
    DELETE - Used to remove data
    PATCH - Used to apply a partial modification of the data

2. What is Sinatra?
    A domain-specific language that is used to write web applications written in ruby and is a library of ruby as well.  It is an alternative to our Ruby on Rails framework.

4. What is MVC?
    Models, Views, Controllers   -  Model contains our data, the view is what the user sees, the controller is how things connect or act.

5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
    To maintain ruby's convention of "easy to read our/others code" when viewing it at any time.

6. What types of variables are accessible in our view templates without explicitly passing them?
    instance variables

7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?

  ```ruby
  get '/horses' do
    @count = Horses.create(params[count: 1])
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?
    <%= @horses.count%> inside our erb file

9. What's the purpose of ERB?
      Embedded ruby code that is able to be rendered along with html to the browser.

10. Why do I need a development AND test database?
      The test database helps you see and make changes before implementing a permanent code set for your tasks at hand.  With constant changing this practice makes things smoother for writing.

11. What's responsive design?
      When viewing the same content on different devices, it is a design to be able to change its paramaters to fit the current device in use.

12. What is CRUD and why is it important?
      Create, Read, Update, Delete.  These are our guidelines too creating and maintaining a database.

13. What does HTTP stand for?
      Hyper Text Transfer Protocol

14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
    <% %> - executes our code, while the interpolated code itself is not seen on the view page
    <%= %> - renders the interpolated code onto the view page

15. What's an ORM?
      Object Relational Mapping - a programming technique capable of converting incompatible type systems in an object-oriented language.  

16. What's the most commonly used ORM in ruby (Sinatra & Rails)?
      ActiveRecord

17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.

    "/restaurants" GET - see all restaurants
    "/restaurants/:id" GET - See single restaurant
    "/restaurants/new" GET - create a restaurant
    "/restaurants" POST - save a restaurant
    "/restaurants/:id/edit" GET - View a form to be able to update a restaurant
    "/restaurants/:id" PUT - Updates data to restaurant
    "/restaurants/:id/edit" DELETE - Removes the restaurant with that id  

18. What's a migration?
      the sending of data from a database to be extracted into set parameters.

19. When you create a migration, does it automatically modify your database?
      yes.

20. How does a model relate to a database?
      Model stores the attributes of a given thing, while the database will fill in the attributes with values.

21. What's the difference between agile workflow and waterfall method?
      Agile is the practice of breaking everything down to the smallest components with constant commits and updates to the pieces of code as progress is made.    Waterfall is about completing a component and seeing how it flows after, than making changes.

22. What is the difference between `#new` and `#create`?
      The new method will require the information to be saved after its fully entered in the database.
      The create method automatically creates and instance and saves it.
