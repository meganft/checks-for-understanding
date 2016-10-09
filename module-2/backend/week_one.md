## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
```
  GET - read data
  POST - insert data
  PUT - update data
  PATCH - update data?
  DELETE - delete data
 ```
  
2. What is Sinatra?
```
  Sinatra is a gem you install that makes it easy to test and host new web applications locally
```
 
4. What is MVC?
```
  Acronym for Model, View, Controller. It's how we structure our apps. 
```

5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
 ```
  To make it easy for other developers to read/understand 
 ```
 
6. What types of variables are accessible in our view templates without explicitly passing them?
  ```
  Instance variables
 ```
  
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    erb :index
  end
  ```

```
Add @count = 1 inside your get '/horses/ loop
```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
  ```
  update the row erb :index to be erb :index, :locals=> {:name => "Mr. Ed"}
  ```

9. What's the purpose of ERB?
```
   It allows us to use ruby code in our HTML view
 ```
  
10. Why do I need a development AND test database?
```
    You need both so that you can test without it impacting your database
  ```

11. What's responsive design?
```
    Design that adapts to different screen sizes 
  ```
  
12. What is CRUD and why is it important?
```
    CRUD stands for create, read, update and delete.  It's important because it represents the basic functions of an application that interacts with a database
  ```
    
13. What does HTTP stand for? 
```
    Hyper Text transfer protocol
  ```
    
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
```
  <%= ruby code %> prints out the code
  <% ruby code %> runs code but doesn't print it
```

15. What's an ORM?
```
  Object relationship mapping
 ```

16. What's the most commonly used ORM?  
```
  Active record?
```

17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
 ```
  get '/restaurants' do   - read
    renders a view of all the restaurants 
  
  get '/restaurants/:id' do   - read
    renders a view of a single restaurant
  
  get '/restaurants/new' do  - create
    renders a new erb template 
  
  post 'restaurants' do  - create
    redirects to the view of restaurants after the user has created a new one
  
  get '/restaurants/:id/edit' do - update
    renders an edit view
  
  post 'restaurants/:id' do -  update
    redirects to the specific restaurant that the user has updated
  
  delete '/restaurants/:id/delete' do  - delete
    redirects to a the restaurants index after the user deletes one
 ```


18. What's a migration? 
```
  A way to run files that will make changes to the database/schema
 ```

19. When you create a migration, does it automatically modify your database?
```
  Only after you run rake db:migrate
 ```
  
20. How does a model relate to a database?
```
  A model represents the table in a database. This is where you have all of your methods.

``
